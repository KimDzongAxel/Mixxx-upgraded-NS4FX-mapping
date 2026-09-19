# NS4FX upgraded mapping for Mixxx

I've made this updated mixxx mapping for NS4FX controller to fix some bugs that are present in the version included with Mixxx 2.6. Original version made by Tomáš Bažant, Erik Puschendorf, Matthew Nicholson is very good and I can't thank those guys enough for the hard work they did but there are some issues in that mapping that made using it difficult (ie. keylock mapping, rate soft takeover not working etc.). After I fixed the bugs I've started adding features I needed that make using this controller easier and give new capabilities not present before (ie. hotcue scrolling on preview deck). Some of those changes are not in line with how the controller is intended to be used (ie. keylock mapped to pitch play mode button) and should be considered work-in-progress meaning I can (and will) change them as I go.

If you want to use it, fork it or help me develop this mapping feel free to do so.

## Bugfixes

If you're looking only for bugfixes there's a branch for you where I've left only fixes to rate soft takeover and missing button definitions.

## Newly added features and changes to original mapping

Some of the features are very much not in line with how the controller should work and will be changed in the future (ie. using Pitch Play as keylock) and other "non standard" features will probably be added in the future (ie. beat grid adjustment options mapped to "roll" pad mode or beat jumping instead of "scratch bank" pad mode). What I'm trying to say is that basically I'm making changes that customize this controller mapping to my needs rather than strictly implementing features as Numark intended.

### List of currrent changes:

- **Keylock remap** - moved keylock enable from pitch bend buttons to pitch play pad mode button
- **Loop anchor remap** - mapped loop anchor control to roll pad mode button. Roll mode button was not used and loop anchor was not mapped to anything I found it useful
- **Preview deck control** - pressing knob button while track is highlighted loads it to preview deck and plays it. Second press stops it (and if selected ejects)
- **Preview deck hotcue scrolling** - if a track is playing on a preview deck then shift + knob turn will jump between cue points in the track so that it's easy to actually preview track without having to use mouse

## Help needed

I'm trying to implement some features but I can't really make them work, if you happen to know how to make them work please send me a message or a PR.

- disable jog wheel innertia in wheel/view mode (it's driving me crazy mad) - PLEASE SEND HELP
  UPDATE - I'm quite sure it's hardcoded into C++ code so I will have to make a change in the mixxx code itself (tbd when)
