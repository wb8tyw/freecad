# General notes for tablet and phone cases

These are initial notes and may not be the same as the final FreeCad
drawings.  See the actual FreeCad or Step files for better measurements

## Generic initial parameters

### Initial Device support sketch and pad

* device_height: 140.60 mm
* device_corner_radius: 8.41 mm
* device_width: 68.5 mm
* device_lip_support: 5.0 mm
* device_center_support: 20.00 mm
* device_support_pad.Length: 8.7 mm

### Initial Case

* device_support_pad_Length: <<device_support_pad>>.Length + 0.5mm
* case_base_pad.Length: 2 mm
* case_side_thickness: Constraints.case_base_pad.Length

### Initial Case Lip

* case_lip: 1.5 mm
* case_lip_pad.Length: 1.4 mm
* case_back_arc: 90 degrees

## Samsung Galaxy Tab A (2017) SM-T380

### SM-T380 Device support sketch and pad

* device_support_pad.Length: 9.0 mm
* device_width: 123.6 mm
* device_height: 212 mm
* device_corner_radius: 8.41 mm
* device_lip_support: 5.0 mm
* device_center_support: 20.00 mm

### SM-T380 Case

* device_support_pad_Length: <<device_support_pad>>.Length + 0.5mm
* case_base_pad.Length: 2 mm
* case_side_thickness: Constraints.case_base_pad.Length

### SM-T380 Case Lip

* case_lip: 4.0 mm
* case_lip_pad.Length: 1.4 mm
* case_back_arc: 90 degrees
* device_height: Sketch.Constraints.device_height +
                   <<case_edge_sketch>>.Constraints.case_side_thickness
* device_width: <<device_support_sketch>>.Constraints.device_width +
                  <<case_edge_sketch>>.Constraints.case_side_thickness

## Samsung Galaxy A11 SM-A115AP - Incomplete and Untested

### SM-A115AP Device support sketch and pad

* device_thickness: 8.9 nnm  (battery is swelling)
* device_width: 76 mm
* device_height: 162 mm
* device_corner_radius: 7.5 mm
* device_corner_arc = 90 degrees

### SM-A115AP Case

* device_support_pad_Length: <<device_support_pad>>.Length + 0.5mm
* case_base_pad.Length: 2 mm
* case_side_thickness: Constraints.case_base_pad.Length

* rear_speaker_width: 9.5 mm
* rear_speaker_height: 11.65 mm
* rear_speaker_y_center: centered on Y axis
* read_speaker_x_from_device_front: 35.77 mm

* rear_camera_y_device_width: 15 mm
* rear_camera_x_device_height: 32 mm
* rear_camera_y_from_device_right_edge: 4.52
* rear_camera_x_from_device_front: 4.30

* rear_flashlight_device_diameter: 3.63 mm
* rear_flashlight_y_from_camera_left: 0 mm
* rear_flashlight_x_from_device_front: 10.64 mm

* top_audio_jack_device_diameter: 4.17 mm
* top_audio_jack_y_from_device_left: 24 mm
* top_audio_jack_z_from device_front: 3.15 mm

* top_mike_device_diameter: 1 mm
* top_mike_y_from_device_right: 17 mm
* top_mike_z_from_device_top: 3.8

* bottom_mike_device_diameter: 1 mm
* bottom_mike_y_from_device_left: 22.5 mm
* bottom_mike_z_from_device_front: 3.8

* bottom_usb_z_device_height: 3.41 mm
* bottom_usb_y_device_width: 9.12 mm
* bottom_usb_y_center: centered on device
* bottom_usb_z_from device_base: 1.56

* bottom_speaker_z_device_height: 3.14 mm
* bottom_speaker_y_device_width: 9.5 mm
* bottom_speaker_y_from_device_right: 13 mm
* bottom_speaker_z_from_device_base: 1.56

* right_volume_x_device_width: 20.8
* right_volume_z_device_height: 1.82
* right_volume_x_from_device_top: 30 mm
* right_volume_z_from_device: 1/2 device_thickness

* right_button_x_device_width: 10.5

### SM-A115APCase Lip

* case_lip: 4.0 mm
* case_lip_pad.Length: 1.4 mm
* case_back_arc: 90 degrees
* device_height: Sketch.Constraints.device_height +
                   <<case_edge_sketch>>.Constraints.case_side_thickness
* device_width: <<device_support_sketch>>.Constraints.device_width +
                  <<case_edge_sketch>>.Constraints.case_side_thickness

## Samsung SMJ337A - Measurements only

### SMJ337A Device support sketch and pad

* device_thickness: 9.19 nnm
* device_width: 70.25 mm
* device_height: 142.36 mm
* device_corner_radius = 8.41 mm
* device_corner_arc = 90 degrees

### SMJ337A Case

* power_width: 12.75 mm
* power_height: 7.0 mm
* power_arc: 90 degrees
* power_corner_radius = 1.25 mm
* power_y_center:Symmetrical on Y axis.
* power_y_bottom: <<case_base_pad>>.Length

* audio_diameter: 6.52 mm
* audio_y_center: 5.12mm + (.Constraints.power_width - .Constraints.audio_diameter) / 2
* audio_z_center: <<case_base_pad>>.Length +
                <<case_edge_sketch>>.Constraints.device_thickness / 2

* bottom_mike_diameter: 3.82 mm
* bottom_mike_y_center: 5.68mm + .Constraints.bottom_mike_diameter / 2
* bottom_mike_z_center: 4.95mm + <<case_base_pad>>.Length

* top_mike_diameter: <<case_bottom_sketch>>.Constraints.bottom_mike_diameter
* top_mike_y_center: 18.30 mm to right edge
* top_mike_z_center: audio_z_lock

* camera_hole_arc: 90 mm
* camera_hole_length: 23.8 mm
* camera_hole_width: 18.0 mm
* camera_hole_y_loc: Symmetrical on X axis
* camera_hole_x_offset_top:  8 mm from case_base_top_edge.

* right_speaker_height: 3.95 mm
* right_speaker_width: 10.55mm - .Constraints.right_speaker_height / 2
* right_speaker_x_offset_top:  14.65mm - .Constraints.right_speaker_height / 2
* right_speaker_base_z_offset: 3.65 mm + <<case_base_pad>>.Length

### SMJ337A Case Lip

* case_lip: 4.0 mm
* case_lip_pad.Length: 1.4 mm
* case_back_arc: 90 degrees
* device_height: Sketch.Constraints.device_height +
                   <<case_edge_sketch>>.Constraints.case_side_thickness
* device_width: <<device_support_sketch>>.Constraints.device_width +
                  <<case_edge_sketch>>.Constraints.case_side_thickness
