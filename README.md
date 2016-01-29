# sne-internal

This repository is used to store datasets that are pulled directly from historical papers that have not yet been digitized. The repository will be different from the other repositories within the OSC in that individual event files will be edited by hand, as older papers do not have actual text objects, just image scans of each page. Each file in this repository should be prefaced with a few comments in their headers describing the data (beginning with the '#' symbol), the goal here is to make the files easily readable with the same Python script.

Ideally, we would want `MJD, Band, Instrument, Magnitude, Error, Upper limit` in that order, but not all supernovae will have this info handy.

Here's an example file for SN1937A:

```JSON
{
  "SN1937A":{
    "sources":[ { "bibcode":"1937PASP...49..204Z" } ],
    "photometry":[
      { "timeunit":"JD", "time":"2428521", "band":"Mp", "abmag":"17.5", "instrument":"18-inch Schmidt", "upperlimit":true },
      { "timeunit":"JD", "time":"2428524", "band":"Mp", "abmag":"17.5", "instrument":"18-inch Schmidt", "upperlimit":true },
      { "timeunit":"JD", "time":"2428581", "band":"Mp", "abmag":"16.2", "instrument":"18-inch Schmidt" },
      { "timeunit":"JD", "time":"2428599", "band":"Mp", "abmag":"16.7", "instrument":"18-inch Schmidt" },
      { "timeunit":"JD", "time":"2428600", "band":"Mp", "abmag":"16.5", "instrument":"18-inch Schmidt" },
      { "timeunit":"JD", "time":"2428635", "band":"Mp", "abmag":"16.9", "instrument":"18-inch Schmidt" },
      { "timeunit":"JD", "time":"2428636", "band":"Mp", "abmag":"17.2", "instrument":"18-inch Schmidt" },
      { "timeunit":"JD", "time":"2428664", "band":"Mp", "abmag":"17.5", "instrument":"18-inch Schmidt", "upperlimit":true },
      { "timeunit":"JD", "time":"2428667", "band":"Mp", "abmag":"19.3", "instrument":"18-inch Schmidt" }
    ]
  }
}
