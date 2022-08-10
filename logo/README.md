About the WTF logo:

I made this inside Keynote, using Hex:

> Hex is a type-able three letter hexagonal monogram font.

Available from many places that distribute free fonts. Such as:

  * <https://www.dafont.com/hex.font>
  * <http://fonts101.com/fonts/view/Gothic/72428/Hex>

Important note about using Hex:

> It requires Discretionary Ligatures to be supported AND enabled to work 'out of the box', so please check the read me pdf for details of how to use it and for useful links to show you applications that support Open Type features it relies on to work (thanks Vinz).

I've included the aforementioned PDF here.

The "iwTf" in the upper right corner of the Keynote is the text you enter to produce the WTF logo, when you apply the Hex font.

I can't remember if I needed to do anything to get discretionary ligatures working.

We seem to have settled on "monograms" style (as opposed to "ornate"), with border 3.

2019-10-23 Anywhere the logo appears as a png or jpeg? For example, as a GitHub avatar. It has been done in a fairly primitive way. I exported the Keynote file to PNG, then manipulated in various low-tech ways. We should probably revisit this.

2022-07 There are images here that claim to have a transparent background that do not. Shannon tackled this in https://github.com/rstats-wtf/wtf-workshop/pull/7 and ultimately just used MS Word to get a transparent background. This process produced logo/wtf-logo-square-transparent.png.

2022-08 Jenny revisited to see if `convert` could be used to get what we wanted. Note there's no particular reason to think this gets a better result than what MS Word produced. But it will be nice to have a snippet of code for this. I found a solution on StackOverflow that seems to have worked.

First, you have to have png not jpeg:

```
convert wtf-logo-monograms-border3.jpg wtf-logo-monograms-border3.png
```

Then you replace the background color using a floodfill approach. This prevents the white *inside* the hex from getting replaced.

```
color=$( convert wtf-logo-monograms-border3.png -format "%[pixel:p{0,0}]" info:- )
convert wtf-logo-monograms-border3.png -alpha off -bordercolor $color -border 1 \
    \( +clone -fuzz 30% -fill none -floodfill +0+0 $color \
       -alpha extract -geometry 200% -blur 0x0.5 \
       -morphology erode square:1 -geometry 50% \) \
    -compose CopyOpacity -composite -shave 1 wtf-logo-monograms-border3-transparent-bg.png
```

> This is rather a bit longer than the simple answers previously given, but it gives much better results: (1) The quality is superior due to antialiased alpha, and (2) only the background is removed as opposed to a single color. ("Background" is defined as approximately the same color as the top left pixel, using a floodfill from the picture edges.)

https://stackoverflow.com/a/44542839

