# Reaper Tools

A collection of customized effects and scripts for [Reaper](https://www.reaper.fm/).

## Download & Install
Download the zip file from [here](https://github.com/samlletas/jsfx/archive/refs/heads/main.zip), extract
it and copy the files into your Reaper folder.

## Effects

### MIDI d'Arpagnan

Modified version of Jahudka's [d'Arpagnan Arpeggiator](https://github.com/jahudka/reaper-consolefx).
I added more patterns with several possible directions each, also removed the backtrack controls
since I didn't use them that much. Velocity is no longer hardcoded and it can be modulated via a LFO.

![midi_darpagnan](https://github.com/samlletas/jsfx/assets/7089504/5a611bbe-d116-4dce-b67c-cc633018c41a)

## Scripts

- **play_selection:** Plays time selection without moving the edit cursor.
- **record_once:** Records a single take and plays the recorded input in the next loop. The script works
best when enabling `Preferences -> Audio -> Loop recording -> "In loop recording, discard incomplete take if at least one loop was recorded"`
- **navigate_home:** Go to start of loop/item/project.
- **navigate_end:** Go to end of loop/item/project.
- **toggle_midi_preview:** Toggle MIDI preview on play/stop (modified version of cfillion's [script](https://github.com/ReaTeam/ReaScripts/blob/master/MIDI%20Editor/cfillion_Toggle%20MIDI%20preview%20on%20transport%20change.lua)).

## Development & Contributing

If a new parameter/slider is needed please add it after the previous ones to avoid breaking compatibility.

### Making Commits
All commits should be made using the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/#summary) specification, to help with this a git hook that validates commit messages can be installed with:

     cp -r -T .githooks .git/hooks
