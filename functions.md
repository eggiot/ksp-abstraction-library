# THE KSP ABSTRACTION LIBRARY
### `kal_init()`


You need to call `kal_init()` in your init callback.
It declares variables that are necessary for the abstraction
library to function

## Volume 
### `change_volume_group(volume, group)`


Change the volume of a single group

- volume: the new volume
- group: the group number

### `change_volume_group_range(volume, first, last)`


Change the volume of a range of groups

- volume: the new volume
- first: the first group in the range
- last: the last group in the range

### `change_tuning_group(tuning, group)`


Change the tuning of a single group

- volume: the new tuning
- group: the group number

### `change_tuning_group_range(tuning, first, last)`


Change the tuning of a range of groups

- volume: the new tuning
- first: the first group in the range
- last: the last group in the range

### `change_cutoff_group(cutoff, group, slot)`


Change the cutoff frequency of a filter in a single group

- cutoff: the new cutoff frequency
- group: the group number
- slot: the filter slot

### `change_resonance_group(resonance, group, slot)`


Change the resonance of a filter in a single group

- resonance: the new resonance
- group: the group number
- slot: the filter slot

### `change_filter_gain_group(gain, group, slot)`


Change the gain of a Ladder or Daft filter in a single group

- gain: the new gain
- group: the group number
- slot: the filter slot

### `change_cutoff_group_range(cutoff, first, last, slot)`


Change the cutoff frequency of a filter in a range of groups

- cutoff: the new cutoff frequency
- group: the group number
- slot: the filter slot

### `change_resonance_group_range(resonance, first, last, slot)`


Change the resonance of a filter in a range of groups

- resonance: the new resonance
- group: the group number
- slot: the filter slot

### `change_filter_gain_group_range(gain, first, last, slot)`


Change the gain of a Ladder or Daft filter in a range of groups

- gain: the new gain
- group: the group number
- slot: the filter slot

### `set_env_hold(name, value, group)`


Change the hold parameter of an AHDSR envelope generator in a single group

- name: the name of the AHDSR envelope generator
- value: the new value of the parameter
- group: the group to change

### `set_env_attack(name, value, group)`


Change the attack parameter of an AHDSR envelope generator in a single group

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- group: the group to change

### `set_env_decay(name, value, group)`


Change the decay parameter of an AHDSR envelope generator in a single group

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- group: the group to change

### `set_env_sustain(name, value, group)`


Change the sustain parameter of an AHDSR envelope generator in a single group

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- group: the group to change

### `set_env_release(name, value, group)`


Change the release parameter of an AHDSR envelope generator in a single group

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- group: the group to change

### `set_env_hold_group_range(name, value, first, last)`


Change the hold parameter of an AHDSR envelope generator in a range of groups.

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- first: the index of the first group in the range
- last: the index of the last group in the range

### `set_env_attack_group_range(name, value, first, last)`


Change the attack parameter of an AHDSR envelope generator in a range of groups.

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- first: the index of the first group in the range
- last: the index of the last group in the range

### `set_env_decay_group_range(name, value, first, last)`


Change the decay parameter of an AHDSR envelope generator in a range of groups.

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- first: the index of the first group in the range
- last: the index of the last group in the range

### `set_env_sustain_group_range(name, value, first, last)`


Change the sustain parameter of an AHDSR envelope generator in a range of groups.

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- first: the index of the first group in the range
- last: the index of the last group in the range

### `set_env_release_group_range(name, value, first, last)`


Change the release parameter of an AHDSR envelope generator in a range of groups.

- name: the name of the AHDSR envelope generator
- value: the new value of the hold parameter
- first: the index of the first group in the range
- last: the index of the last group in the range

### `set_lfo_sine(name, value, group)`
## LFOs 
### `set_lfo_tri(name, value, group)`
### `set_lfo_rect(name, value, group)`
### `set_lfo_saw(name, value, group)`
### `set_lfo_rand(name, value, group)`
### `set_lfo_pulse(name, value, group)`
### `set_lfo_frequency(name, value, group)`
### `change_group_int_target_intensity(value, mod_name, target_name, group)`


Changes the modulation intensity of an internal modulation strip in a single group

- value: the new target intensity
- mod_name: the name of the modulator
- target_name: the name of the modulation strip
- group: the group we will be affecting

### `change_groups_int_target_intensity(value, mod_name, target_name, first, last)`


Changes the modulation intensity of an internal modulation strip in a range of groups

- value: the new target intensity
- mod_name: the name of the modulator
- target_name: the name of the modulation strip
- first: the index of the first group in the range
- last: the index of the last group in the range

### `change_group_ext_target_intensity(value, target_name, group)`


Changes the modulation intensity of an external modulation strip in a single group

- value: the new modulation intensity
- target_name: the name of the modulation strip
- group: the group we will be affecting

### `change_groups_ext_target_intensity(value, target_name, first, last)`


Changes the modulation intensity of an external modulation strip in a range of groups

- value: the new target intensity
- target_name: the name of the modulation strip
- first: the index of the first group in the range
- last: the index of the last group in the range

### `change_group_int_target_intensity_bipolar(value, mod_name, target_name, group)`


Changes the modulation intensity of an internal modulation strip in a single group
so that the intensity is bipolar (i.e. has a negative and positive extreme)

- value: the new target intensity
- mod_name: the name of the modulator
- target_name: the name of the modulation strip
- group: the group we will be affecting

### `change_groups_int_target_intensity_bipolar(value, mod_name, target_name, first, last)`


Changes the modulation intensity of an internal modulation strip in a range of groups
so that the intensity is bipolar (i.e. has a negative and positive extreme)

- value: the new target intensity
- mod_name: the name of the modulator
- target_name: the name of the modulation strip
- first: the index of the first group in the range
- last: the index of the last group in the range

### `change_group_ext_target_intensity_bipolar(value, target_name, group)`


Changes the modulation intensity of an external modulation strip in a single group
so that the intensity is bipolar (i.e. has a negative and positive extreme)

- value: the new modulation intensity
- target_name: the name of the modulation strip
- group: the group we will be affecting

### `change_groups_ext_target_intensity_bipolar(value, target_name, first, last)`


Changes the modulation intensity of an external modulation strip in a range of groups
so that the intensity is bipolar (i.e. has a negative and positive extreme)

- value: the new target intensity
- target_name: the name of the modulation strip
- first: the index of the first group in the range
- last: the index of the last group in the range

### `set_wallpaper(image)`


Set the wallpaper

- image: a character string containing the file name of the image (without extension)

### `make_custom_knob(variable, image, min_value, max_value, x, y)`


Make a knob with a custom graphic and display it in the UI.

- variable: the name of the knob variable we will create
- image: a character string containing the file name of the image (without extension)
- min_value: the minimum value of the knob
- max_value: the maximum value of the knob
- x: the horizontal location of the knob within the UI
- y: the vertical location of the knob within the UI

### `make_image_label(variable, image, x, y)`


Make a label with a custom graphic and display it in the UI.

- variable: the name of the label variable we will create
- image: a character string containing the file name of the image (without extension)
- x: the horizontal location of the label within the UI
- y: the vertical location of the label within the UI

### `make_custom_button(variable, image, x, y)`


Make a button with a custom graphic and display it in the UI.

- variable: the name of the button variable we will create
- image: a character string containing the file name of the image (without extension)
- x: the horizontal location of the button within the UI
- y: the vertical location of the button within the UI

### `set_instrument_icon(image)`


Set the instrument icon image

- image: a character string containing the file name of the image (without extension)

### `grid_coord(position, slots, offset, size) -> result`


Get an x or y coordinate in a grid system

- position: the grid position of which we want the coordinate
- slots: the number of slots in the grid
- offset: an offset to add on to the slot coordinate
- size: the size in pixels of the grid

### `horizontal_grid_coord(position, slots, offset) -> result`


Get an x coordinate in a grid system

- position: the grid position of which we want the coordinate
- slots: the number of slots in the grid
- offset: an offset to add on to the slot coordinate

### `set_automation_name(variable, name)`
## Automation 
### `enable_automation(variable)`
### `disable_automation(variable)`
### `sep_group_range(parameter, value, first, last, slot, generic)`
## Abstraction library abstractions 
### `sep_target_group_range(parameter, value, first, last, target_name, generic)`