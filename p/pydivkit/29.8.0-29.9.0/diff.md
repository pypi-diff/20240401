# Comparing `tmp/pydivkit-29.8.0.tar.gz` & `tmp/pydivkit-29.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivkit-29.8.0.tar", max compression
+gzip compressed data, was "pydivkit-29.9.0.tar", max compression
```

## Comparing `pydivkit-29.8.0.tar` & `pydivkit-29.9.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0     9446 2024-02-26 12:25:59.286784 pydivkit-29.8.0/README.md
--rw-r--r--   0        0        0      700 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/__init__.py
--rw-r--r--   0        0        0      164 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/core/__init__.py
--rw-r--r--   0        0        0      445 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/core/compat.py
--rw-r--r--   0        0        0    28631 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/core/entities.py
--rw-r--r--   0        0        0     3039 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/core/fields.py
--rw-r--r--   0        0        0        0 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/core/types/__init__.py
--rw-r--r--   0        0        0      728 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/core/types/union.py
--rw-r--r--   0        0        0    16462 2024-02-26 12:26:49.813457 pydivkit-29.8.0/pydivkit/div/__init__.py
--rw-r--r--   0        0        0      611 2024-02-26 12:26:49.537727 pydivkit-29.8.0/pydivkit/div/array_value.py
--rw-r--r--   0        0        0      857 2024-02-26 12:26:49.535427 pydivkit-29.8.0/pydivkit/div/array_variable.py
--rw-r--r--   0        0        0      613 2024-02-26 12:26:49.534125 pydivkit-29.8.0/pydivkit/div/boolean_value.py
--rw-r--r--   0        0        0      861 2024-02-26 12:26:49.539396 pydivkit-29.8.0/pydivkit/div/boolean_variable.py
--rw-r--r--   0        0        0      627 2024-02-26 12:26:49.535810 pydivkit-29.8.0/pydivkit/div/color_value.py
--rw-r--r--   0        0        0      875 2024-02-26 12:26:49.535802 pydivkit-29.8.0/pydivkit/div/color_variable.py
--rw-r--r--   0        0        0      603 2024-02-26 12:26:49.537406 pydivkit-29.8.0/pydivkit/div/content_text.py
--rw-r--r--   0        0        0      621 2024-02-26 12:26:49.537775 pydivkit-29.8.0/pydivkit/div/content_url.py
--rw-r--r--   0        0        0      609 2024-02-26 12:26:49.546062 pydivkit-29.8.0/pydivkit/div/dict_value.py
--rw-r--r--   0        0        0      856 2024-02-26 12:26:49.548776 pydivkit-29.8.0/pydivkit/div/dict_variable.py
--rw-r--r--   0        0        0      863 2024-02-26 12:26:49.546061 pydivkit-29.8.0/pydivkit/div/div.py
--rw-r--r--   0        0        0     1209 2024-02-26 12:26:49.546617 pydivkit-29.8.0/pydivkit/div/div_absolute_edge_insets.py
--rw-r--r--   0        0        0     3234 2024-02-26 12:26:49.558823 pydivkit-29.8.0/pydivkit/div/div_accessibility.py
--rw-r--r--   0        0        0     4162 2024-02-26 12:26:49.562318 pydivkit-29.8.0/pydivkit/div/div_action.py
--rw-r--r--   0        0        0     1057 2024-02-26 12:26:49.551093 pydivkit-29.8.0/pydivkit/div/div_action_array_insert_value.py
--rw-r--r--   0        0        0      863 2024-02-26 12:26:49.550736 pydivkit-29.8.0/pydivkit/div/div_action_array_remove_value.py
--rw-r--r--   0        0        0      837 2024-02-26 12:26:49.556106 pydivkit-29.8.0/pydivkit/div/div_action_copy_to_clipboard.py
--rw-r--r--   0        0        0      346 2024-02-26 12:26:49.554140 pydivkit-29.8.0/pydivkit/div/div_action_copy_to_clipboard_content.py
--rw-r--r--   0        0        0      732 2024-02-26 12:26:49.558389 pydivkit-29.8.0/pydivkit/div/div_action_focus_element.py
--rw-r--r--   0        0        0      885 2024-02-26 12:26:49.559666 pydivkit-29.8.0/pydivkit/div/div_action_set_variable.py
--rw-r--r--   0        0        0      687 2024-02-26 12:26:49.557916 pydivkit-29.8.0/pydivkit/div/div_action_typed.py
--rw-r--r--   0        0        0      321 2024-02-26 12:26:49.559547 pydivkit-29.8.0/pydivkit/div/div_alignment_horizontal.py
--rw-r--r--   0        0        0      309 2024-02-26 12:26:49.563633 pydivkit-29.8.0/pydivkit/div/div_alignment_vertical.py
--rw-r--r--   0        0        0     3016 2024-02-26 12:26:49.573486 pydivkit-29.8.0/pydivkit/div/div_animation.py
--rw-r--r--   0        0        0      371 2024-02-26 12:26:49.566075 pydivkit-29.8.0/pydivkit/div/div_animation_interpolator.py
--rw-r--r--   0        0        0      879 2024-02-26 12:26:49.569397 pydivkit-29.8.0/pydivkit/div/div_appearance_set_transition.py
--rw-r--r--   0        0        0      557 2024-02-26 12:26:49.565536 pydivkit-29.8.0/pydivkit/div/div_appearance_transition.py
--rw-r--r--   0        0        0      671 2024-02-26 12:26:49.566800 pydivkit-29.8.0/pydivkit/div/div_aspect.py
--rw-r--r--   0        0        0      599 2024-02-26 12:26:49.566149 pydivkit-29.8.0/pydivkit/div/div_background.py
--rw-r--r--   0        0        0     9678 2024-02-26 12:26:49.588630 pydivkit-29.8.0/pydivkit/div/div_base.py
--rw-r--r--   0        0        0      369 2024-02-26 12:26:49.571555 pydivkit-29.8.0/pydivkit/div/div_blend_mode.py
--rw-r--r--   0        0        0      764 2024-02-26 12:26:49.578188 pydivkit-29.8.0/pydivkit/div/div_blur.py
--rw-r--r--   0        0        0     1734 2024-02-26 12:26:49.576583 pydivkit-29.8.0/pydivkit/div/div_border.py
--rw-r--r--   0        0        0     1403 2024-02-26 12:26:49.582626 pydivkit-29.8.0/pydivkit/div/div_change_bounds_transition.py
--rw-r--r--   0        0        0      809 2024-02-26 12:26:49.580104 pydivkit-29.8.0/pydivkit/div/div_change_set_transition.py
--rw-r--r--   0        0        0      420 2024-02-26 12:26:49.576195 pydivkit-29.8.0/pydivkit/div/div_change_transition.py
--rw-r--r--   0        0        0     1176 2024-02-26 12:26:49.585210 pydivkit-29.8.0/pydivkit/div/div_circle_shape.py
--rw-r--r--   0        0        0     2552 2024-02-26 12:26:49.583714 pydivkit-29.8.0/pydivkit/div/div_collection_item_builder.py
--rw-r--r--   0        0        0    18193 2024-02-26 12:26:49.635556 pydivkit-29.8.0/pydivkit/div/div_container.py
--rw-r--r--   0        0        0      432 2024-02-26 12:26:49.587427 pydivkit-29.8.0/pydivkit/div/div_content_alignment_horizontal.py
--rw-r--r--   0        0        0      420 2024-02-26 12:26:49.588125 pydivkit-29.8.0/pydivkit/div/div_content_alignment_vertical.py
--rw-r--r--   0        0        0     1861 2024-02-26 12:26:49.593879 pydivkit-29.8.0/pydivkit/div/div_corners_radius.py
--rw-r--r--   0        0        0      351 2024-02-26 12:26:49.588756 pydivkit-29.8.0/pydivkit/div/div_count.py
--rw-r--r--   0        0        0     1246 2024-02-26 12:26:49.596492 pydivkit-29.8.0/pydivkit/div/div_currency_input_mask.py
--rw-r--r--   0        0        0    10575 2024-02-26 12:26:49.623746 pydivkit-29.8.0/pydivkit/div/div_custom.py
--rw-r--r--   0        0        0     2826 2024-02-26 12:26:49.601167 pydivkit-29.8.0/pydivkit/div/div_data.py
--rw-r--r--   0        0        0      872 2024-02-26 12:26:49.597611 pydivkit-29.8.0/pydivkit/div/div_default_indicator_item_placement.py
--rw-r--r--   0        0        0      802 2024-02-26 12:26:49.598385 pydivkit-29.8.0/pydivkit/div/div_dimension.py
--rw-r--r--   0        0        0     3528 2024-02-26 12:26:49.605906 pydivkit-29.8.0/pydivkit/div/div_disappear_action.py
--rw-r--r--   0        0        0     1184 2024-02-26 12:26:49.603223 pydivkit-29.8.0/pydivkit/div/div_download_callbacks.py
--rw-r--r--   0        0        0      302 2024-02-26 12:26:49.602618 pydivkit-29.8.0/pydivkit/div/div_drawable.py
--rw-r--r--   0        0        0     2081 2024-02-26 12:26:49.609477 pydivkit-29.8.0/pydivkit/div/div_edge_insets.py
--rw-r--r--   0        0        0      804 2024-02-26 12:26:49.608209 pydivkit-29.8.0/pydivkit/div/div_extension.py
--rw-r--r--   0        0        0     1675 2024-02-26 12:26:49.617250 pydivkit-29.8.0/pydivkit/div/div_fade_transition.py
--rw-r--r--   0        0        0      340 2024-02-26 12:26:49.610908 pydivkit-29.8.0/pydivkit/div/div_filter.py
--rw-r--r--   0        0        0      564 2024-02-26 12:26:49.613621 pydivkit-29.8.0/pydivkit/div/div_filter_rtl_mirror.py
--rw-r--r--   0        0        0      686 2024-02-26 12:26:49.621803 pydivkit-29.8.0/pydivkit/div/div_fixed_count.py
--rw-r--r--   0        0        0     3267 2024-02-26 12:26:49.631545 pydivkit-29.8.0/pydivkit/div/div_fixed_length_input_mask.py
--rw-r--r--   0        0        0     1090 2024-02-26 12:26:49.625604 pydivkit-29.8.0/pydivkit/div/div_fixed_size.py
--rw-r--r--   0        0        0     2850 2024-02-26 12:26:49.627245 pydivkit-29.8.0/pydivkit/div/div_focus.py
--rw-r--r--   0        0        0      300 2024-02-26 12:26:49.621092 pydivkit-29.8.0/pydivkit/div/div_font_weight.py
--rw-r--r--   0        0        0    15161 2024-02-26 12:26:49.658695 pydivkit-29.8.0/pydivkit/div/div_gallery.py
--rw-r--r--   0        0        0    14187 2024-02-26 12:26:49.665129 pydivkit-29.8.0/pydivkit/div/div_gif_image.py
--rw-r--r--   0        0        0    12660 2024-02-26 12:26:49.673521 pydivkit-29.8.0/pydivkit/div/div_grid.py
--rw-r--r--   0        0        0    15911 2024-02-26 12:26:49.677003 pydivkit-29.8.0/pydivkit/div/div_image.py
--rw-r--r--   0        0        0     2530 2024-02-26 12:26:49.641245 pydivkit-29.8.0/pydivkit/div/div_image_background.py
--rw-r--r--   0        0        0      300 2024-02-26 12:26:49.639388 pydivkit-29.8.0/pydivkit/div/div_image_scale.py
--rw-r--r--   0        0        0    13843 2024-02-26 12:26:49.670515 pydivkit-29.8.0/pydivkit/div/div_indicator.py
--rw-r--r--   0        0        0      490 2024-02-26 12:26:49.640408 pydivkit-29.8.0/pydivkit/div/div_indicator_item_placement.py
--rw-r--r--   0        0        0      516 2024-02-26 12:26:49.647086 pydivkit-29.8.0/pydivkit/div/div_infinity_count.py
--rw-r--r--   0        0        0    16212 2024-02-26 12:26:49.685747 pydivkit-29.8.0/pydivkit/div/div_input.py
--rw-r--r--   0        0        0      478 2024-02-26 12:26:49.646727 pydivkit-29.8.0/pydivkit/div/div_input_mask.py
--rw-r--r--   0        0        0      648 2024-02-26 12:26:49.653335 pydivkit-29.8.0/pydivkit/div/div_input_mask_base.py
--rw-r--r--   0        0        0      424 2024-02-26 12:26:49.652868 pydivkit-29.8.0/pydivkit/div/div_input_validator.py
--rw-r--r--   0        0        0     1277 2024-02-26 12:26:49.662470 pydivkit-29.8.0/pydivkit/div/div_input_validator_base.py
--rw-r--r--   0        0        0     1719 2024-02-26 12:26:49.667022 pydivkit-29.8.0/pydivkit/div/div_input_validator_expression.py
--rw-r--r--   0        0        0     1628 2024-02-26 12:26:49.669407 pydivkit-29.8.0/pydivkit/div/div_input_validator_regex.py
--rw-r--r--   0        0        0      255 2024-02-26 12:26:49.671522 pydivkit-29.8.0/pydivkit/div/div_line_style.py
--rw-r--r--   0        0        0     1046 2024-02-26 12:26:49.675115 pydivkit-29.8.0/pydivkit/div/div_linear_gradient.py
--rw-r--r--   0        0        0      974 2024-02-26 12:26:49.676423 pydivkit-29.8.0/pydivkit/div/div_match_parent_size.py
--rw-r--r--   0        0        0      858 2024-02-26 12:26:49.677744 pydivkit-29.8.0/pydivkit/div/div_neighbour_page_size.py
--rw-r--r--   0        0        0     1297 2024-02-26 12:26:49.679876 pydivkit-29.8.0/pydivkit/div/div_nine_patch_background.py
--rw-r--r--   0        0        0      795 2024-02-26 12:26:49.679887 pydivkit-29.8.0/pydivkit/div/div_page_size.py
--rw-r--r--   0        0        0    13227 2024-02-26 12:26:49.708679 pydivkit-29.8.0/pydivkit/div/div_pager.py
--rw-r--r--   0        0        0      369 2024-02-26 12:26:49.679719 pydivkit-29.8.0/pydivkit/div/div_pager_layout_mode.py
--rw-r--r--   0        0        0     1928 2024-02-26 12:26:49.688365 pydivkit-29.8.0/pydivkit/div/div_patch.py
--rw-r--r--   0        0        0      694 2024-02-26 12:26:49.685231 pydivkit-29.8.0/pydivkit/div/div_percentage_size.py
--rw-r--r--   0        0        0      820 2024-02-26 12:26:49.686313 pydivkit-29.8.0/pydivkit/div/div_phone_input_mask.py
--rw-r--r--   0        0        0      357 2024-02-26 12:26:49.684922 pydivkit-29.8.0/pydivkit/div/div_pivot.py
--rw-r--r--   0        0        0     1136 2024-02-26 12:26:49.691275 pydivkit-29.8.0/pydivkit/div/div_pivot_fixed.py
--rw-r--r--   0        0        0      800 2024-02-26 12:26:49.690456 pydivkit-29.8.0/pydivkit/div/div_pivot_percentage.py
--rw-r--r--   0        0        0      768 2024-02-26 12:26:49.692252 pydivkit-29.8.0/pydivkit/div/div_point.py
--rw-r--r--   0        0        0     1933 2024-02-26 12:26:49.697419 pydivkit-29.8.0/pydivkit/div/div_radial_gradient.py
--rw-r--r--   0        0        0      473 2024-02-26 12:26:49.691824 pydivkit-29.8.0/pydivkit/div/div_radial_gradient_center.py
--rw-r--r--   0        0        0     1156 2024-02-26 12:26:49.696639 pydivkit-29.8.0/pydivkit/div/div_radial_gradient_fixed_center.py
--rw-r--r--   0        0        0      412 2024-02-26 12:26:49.693306 pydivkit-29.8.0/pydivkit/div/div_radial_gradient_radius.py
--rw-r--r--   0        0        0      800 2024-02-26 12:26:49.699172 pydivkit-29.8.0/pydivkit/div/div_radial_gradient_relative_center.py
--rw-r--r--   0        0        0     1052 2024-02-26 12:26:49.700736 pydivkit-29.8.0/pydivkit/div/div_radial_gradient_relative_radius.py
--rw-r--r--   0        0        0     1721 2024-02-26 12:26:49.705112 pydivkit-29.8.0/pydivkit/div/div_rounded_rectangle_shape.py
--rw-r--r--   0        0        0     2300 2024-02-26 12:26:49.706726 pydivkit-29.8.0/pydivkit/div/div_scale_transition.py
--rw-r--r--   0        0        0    13666 2024-02-26 12:26:49.731624 pydivkit-29.8.0/pydivkit/div/div_select.py
--rw-r--r--   0        0        0    12833 2024-02-26 12:26:49.734698 pydivkit-29.8.0/pydivkit/div/div_separator.py
--rw-r--r--   0        0        0     1198 2024-02-26 12:26:49.705105 pydivkit-29.8.0/pydivkit/div/div_shadow.py
--rw-r--r--   0        0        0      380 2024-02-26 12:26:49.704194 pydivkit-29.8.0/pydivkit/div/div_shape.py
--rw-r--r--   0        0        0     1144 2024-02-26 12:26:49.711022 pydivkit-29.8.0/pydivkit/div/div_shape_drawable.py
--rw-r--r--   0        0        0     2723 2024-02-26 12:26:49.715344 pydivkit-29.8.0/pydivkit/div/div_sight_action.py
--rw-r--r--   0        0        0      424 2024-02-26 12:26:49.711807 pydivkit-29.8.0/pydivkit/div/div_size.py
--rw-r--r--   0        0        0      256 2024-02-26 12:26:49.713674 pydivkit-29.8.0/pydivkit/div/div_size_unit.py
--rw-r--r--   0        0        0     2360 2024-02-26 12:26:49.720056 pydivkit-29.8.0/pydivkit/div/div_slide_transition.py
--rw-r--r--   0        0        0    16427 2024-02-26 12:26:49.752927 pydivkit-29.8.0/pydivkit/div/div_slider.py
--rw-r--r--   0        0        0      700 2024-02-26 12:26:49.719788 pydivkit-29.8.0/pydivkit/div/div_solid_background.py
--rw-r--r--   0        0        0    13669 2024-02-26 12:26:49.754085 pydivkit-29.8.0/pydivkit/div/div_state.py
--rw-r--r--   0        0        0     1101 2024-02-26 12:26:49.723726 pydivkit-29.8.0/pydivkit/div/div_stretch_indicator_item_placement.py
--rw-r--r--   0        0        0     1000 2024-02-26 12:26:49.725765 pydivkit-29.8.0/pydivkit/div/div_stroke.py
--rw-r--r--   0        0        0    20352 2024-02-26 12:26:49.770545 pydivkit-29.8.0/pydivkit/div/div_tabs.py
--rw-r--r--   0        0        0    25985 2024-02-26 12:26:49.829185 pydivkit-29.8.0/pydivkit/div/div_text.py
--rw-r--r--   0        0        0      373 2024-02-26 12:26:49.729422 pydivkit-29.8.0/pydivkit/div/div_text_gradient.py
--rw-r--r--   0        0        0      319 2024-02-26 12:26:49.733252 pydivkit-29.8.0/pydivkit/div/div_text_range_background.py
--rw-r--r--   0        0        0      975 2024-02-26 12:26:49.738460 pydivkit-29.8.0/pydivkit/div/div_text_range_border.py
--rw-r--r--   0        0        0     2706 2024-02-26 12:26:49.741324 pydivkit-29.8.0/pydivkit/div/div_timer.py
--rw-r--r--   0        0        0     2922 2024-02-26 12:26:49.749475 pydivkit-29.8.0/pydivkit/div/div_tooltip.py
--rw-r--r--   0        0        0     1171 2024-02-26 12:26:49.744444 pydivkit-29.8.0/pydivkit/div/div_transform.py
--rw-r--r--   0        0        0     1234 2024-02-26 12:26:49.751199 pydivkit-29.8.0/pydivkit/div/div_transition_base.py
--rw-r--r--   0        0        0      338 2024-02-26 12:26:49.752617 pydivkit-29.8.0/pydivkit/div/div_transition_selector.py
--rw-r--r--   0        0        0      333 2024-02-26 12:26:49.753544 pydivkit-29.8.0/pydivkit/div/div_transition_trigger.py
--rw-r--r--   0        0        0     1581 2024-02-26 12:26:49.760013 pydivkit-29.8.0/pydivkit/div/div_trigger.py
--rw-r--r--   0        0        0      593 2024-02-26 12:26:49.758536 pydivkit-29.8.0/pydivkit/div/div_typed_value.py
--rw-r--r--   0        0        0      663 2024-02-26 12:26:49.758894 pydivkit-29.8.0/pydivkit/div/div_variable.py
--rw-r--r--   0        0        0    14446 2024-02-26 12:26:49.790624 pydivkit-29.8.0/pydivkit/div/div_video.py
--rw-r--r--   0        0        0      276 2024-02-26 12:26:49.760775 pydivkit-29.8.0/pydivkit/div/div_video_scale.py
--rw-r--r--   0        0        0     2331 2024-02-26 12:26:49.766390 pydivkit-29.8.0/pydivkit/div/div_video_source.py
--rw-r--r--   0        0        0      286 2024-02-26 12:26:49.766409 pydivkit-29.8.0/pydivkit/div/div_visibility.py
--rw-r--r--   0        0        0     3514 2024-02-26 12:26:49.775128 pydivkit-29.8.0/pydivkit/div/div_visibility_action.py
--rw-r--r--   0        0        0     2298 2024-02-26 12:26:49.772260 pydivkit-29.8.0/pydivkit/div/div_wrap_content_size.py
--rw-r--r--   0        0        0      611 2024-02-26 12:26:49.768867 pydivkit-29.8.0/pydivkit/div/integer_value.py
--rw-r--r--   0        0        0      843 2024-02-26 12:26:49.775460 pydivkit-29.8.0/pydivkit/div/integer_variable.py
--rw-r--r--   0        0        0      611 2024-02-26 12:26:49.775086 pydivkit-29.8.0/pydivkit/div/number_value.py
--rw-r--r--   0        0        0      849 2024-02-26 12:26:49.778770 pydivkit-29.8.0/pydivkit/div/number_variable.py
--rw-r--r--   0        0        0      607 2024-02-26 12:26:49.780083 pydivkit-29.8.0/pydivkit/div/string_value.py
--rw-r--r--   0        0        0      837 2024-02-26 12:26:49.781152 pydivkit-29.8.0/pydivkit/div/string_variable.py
--rw-r--r--   0        0        0      617 2024-02-26 12:26:49.783603 pydivkit-29.8.0/pydivkit/div/url_value.py
--rw-r--r--   0        0        0      859 2024-02-26 12:26:49.784124 pydivkit-29.8.0/pydivkit/div/url_variable.py
--rw-r--r--   0        0        0        0 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pydivkit/py.typed
--rw-r--r--   0        0        0     1697 2024-02-26 12:25:59.286784 pydivkit-29.8.0/pyproject.toml
--rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-29.8.0/PKG-INFO
+-rw-r--r--   0        0        0     9446 2024-03-11 13:51:44.836531 pydivkit-29.9.0/README.md
+-rw-r--r--   0        0        0      700 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/__init__.py
+-rw-r--r--   0        0        0      164 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/__init__.py
+-rw-r--r--   0        0        0      445 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/compat.py
+-rw-r--r--   0        0        0    28631 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/entities.py
+-rw-r--r--   0        0        0     3039 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/fields.py
+-rw-r--r--   0        0        0        0 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/types/__init__.py
+-rw-r--r--   0        0        0      728 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/core/types/union.py
+-rw-r--r--   0        0        0    16462 2024-03-11 13:52:24.445063 pydivkit-29.9.0/pydivkit/div/__init__.py
+-rw-r--r--   0        0        0      611 2024-03-11 13:52:24.249505 pydivkit-29.9.0/pydivkit/div/array_value.py
+-rw-r--r--   0        0        0      857 2024-03-11 13:52:24.249608 pydivkit-29.9.0/pydivkit/div/array_variable.py
+-rw-r--r--   0        0        0      613 2024-03-11 13:52:24.249614 pydivkit-29.9.0/pydivkit/div/boolean_value.py
+-rw-r--r--   0        0        0      861 2024-03-11 13:52:24.249701 pydivkit-29.9.0/pydivkit/div/boolean_variable.py
+-rw-r--r--   0        0        0      627 2024-03-11 13:52:24.249480 pydivkit-29.9.0/pydivkit/div/color_value.py
+-rw-r--r--   0        0        0      875 2024-03-11 13:52:24.249639 pydivkit-29.9.0/pydivkit/div/color_variable.py
+-rw-r--r--   0        0        0      603 2024-03-11 13:52:24.249522 pydivkit-29.9.0/pydivkit/div/content_text.py
+-rw-r--r--   0        0        0      621 2024-03-11 13:52:24.249686 pydivkit-29.9.0/pydivkit/div/content_url.py
+-rw-r--r--   0        0        0      609 2024-03-11 13:52:24.255942 pydivkit-29.9.0/pydivkit/div/dict_value.py
+-rw-r--r--   0        0        0      856 2024-03-11 13:52:24.256851 pydivkit-29.9.0/pydivkit/div/dict_variable.py
+-rw-r--r--   0        0        0      863 2024-03-11 13:52:24.255542 pydivkit-29.9.0/pydivkit/div/div.py
+-rw-r--r--   0        0        0     1209 2024-03-11 13:52:24.256182 pydivkit-29.9.0/pydivkit/div/div_absolute_edge_insets.py
+-rw-r--r--   0        0        0     3234 2024-03-11 13:52:24.261068 pydivkit-29.9.0/pydivkit/div/div_accessibility.py
+-rw-r--r--   0        0        0     4162 2024-03-11 13:52:24.264237 pydivkit-29.9.0/pydivkit/div/div_action.py
+-rw-r--r--   0        0        0     1057 2024-03-11 13:52:24.257484 pydivkit-29.9.0/pydivkit/div/div_action_array_insert_value.py
+-rw-r--r--   0        0        0      863 2024-03-11 13:52:24.256452 pydivkit-29.9.0/pydivkit/div/div_action_array_remove_value.py
+-rw-r--r--   0        0        0      837 2024-03-11 13:52:24.261876 pydivkit-29.9.0/pydivkit/div/div_action_copy_to_clipboard.py
+-rw-r--r--   0        0        0      346 2024-03-11 13:52:24.260172 pydivkit-29.9.0/pydivkit/div/div_action_copy_to_clipboard_content.py
+-rw-r--r--   0        0        0      732 2024-03-11 13:52:24.262290 pydivkit-29.9.0/pydivkit/div/div_action_focus_element.py
+-rw-r--r--   0        0        0      885 2024-03-11 13:52:24.263241 pydivkit-29.9.0/pydivkit/div/div_action_set_variable.py
+-rw-r--r--   0        0        0      687 2024-03-11 13:52:24.261478 pydivkit-29.9.0/pydivkit/div/div_action_typed.py
+-rw-r--r--   0        0        0      321 2024-03-11 13:52:24.262761 pydivkit-29.9.0/pydivkit/div/div_alignment_horizontal.py
+-rw-r--r--   0        0        0      309 2024-03-11 13:52:24.265280 pydivkit-29.9.0/pydivkit/div/div_alignment_vertical.py
+-rw-r--r--   0        0        0     3016 2024-03-11 13:52:24.271683 pydivkit-29.9.0/pydivkit/div/div_animation.py
+-rw-r--r--   0        0        0      371 2024-03-11 13:52:24.266235 pydivkit-29.9.0/pydivkit/div/div_animation_interpolator.py
+-rw-r--r--   0        0        0      879 2024-03-11 13:52:24.268551 pydivkit-29.9.0/pydivkit/div/div_appearance_set_transition.py
+-rw-r--r--   0        0        0      557 2024-03-11 13:52:24.265792 pydivkit-29.9.0/pydivkit/div/div_appearance_transition.py
+-rw-r--r--   0        0        0      671 2024-03-11 13:52:24.267263 pydivkit-29.9.0/pydivkit/div/div_aspect.py
+-rw-r--r--   0        0        0      599 2024-03-11 13:52:24.267030 pydivkit-29.9.0/pydivkit/div/div_background.py
+-rw-r--r--   0        0        0     9678 2024-03-11 13:52:24.279948 pydivkit-29.9.0/pydivkit/div/div_base.py
+-rw-r--r--   0        0        0      369 2024-03-11 13:52:24.270048 pydivkit-29.9.0/pydivkit/div/div_blend_mode.py
+-rw-r--r--   0        0        0      764 2024-03-11 13:52:24.272387 pydivkit-29.9.0/pydivkit/div/div_blur.py
+-rw-r--r--   0        0        0     1734 2024-03-11 13:52:24.272606 pydivkit-29.9.0/pydivkit/div/div_border.py
+-rw-r--r--   0        0        0     1403 2024-03-11 13:52:24.275608 pydivkit-29.9.0/pydivkit/div/div_change_bounds_transition.py
+-rw-r--r--   0        0        0      809 2024-03-11 13:52:24.274496 pydivkit-29.9.0/pydivkit/div/div_change_set_transition.py
+-rw-r--r--   0        0        0      420 2024-03-11 13:52:24.272220 pydivkit-29.9.0/pydivkit/div/div_change_transition.py
+-rw-r--r--   0        0        0     1176 2024-03-11 13:52:24.277227 pydivkit-29.9.0/pydivkit/div/div_circle_shape.py
+-rw-r--r--   0        0        0     2552 2024-03-11 13:52:24.278176 pydivkit-29.9.0/pydivkit/div/div_collection_item_builder.py
+-rw-r--r--   0        0        0    18193 2024-03-11 13:52:24.308836 pydivkit-29.9.0/pydivkit/div/div_container.py
+-rw-r--r--   0        0        0      432 2024-03-11 13:52:24.278029 pydivkit-29.9.0/pydivkit/div/div_content_alignment_horizontal.py
+-rw-r--r--   0        0        0      420 2024-03-11 13:52:24.278552 pydivkit-29.9.0/pydivkit/div/div_content_alignment_vertical.py
+-rw-r--r--   0        0        0     1861 2024-03-11 13:52:24.282521 pydivkit-29.9.0/pydivkit/div/div_corners_radius.py
+-rw-r--r--   0        0        0      351 2024-03-11 13:52:24.279674 pydivkit-29.9.0/pydivkit/div/div_count.py
+-rw-r--r--   0        0        0     1246 2024-03-11 13:52:24.283896 pydivkit-29.9.0/pydivkit/div/div_currency_input_mask.py
+-rw-r--r--   0        0        0    10575 2024-03-11 13:52:24.302763 pydivkit-29.9.0/pydivkit/div/div_custom.py
+-rw-r--r--   0        0        0     2826 2024-03-11 13:52:24.285976 pydivkit-29.9.0/pydivkit/div/div_data.py
+-rw-r--r--   0        0        0      872 2024-03-11 13:52:24.286182 pydivkit-29.9.0/pydivkit/div/div_default_indicator_item_placement.py
+-rw-r--r--   0        0        0      802 2024-03-11 13:52:24.285295 pydivkit-29.9.0/pydivkit/div/div_dimension.py
+-rw-r--r--   0        0        0     3528 2024-03-11 13:52:24.290975 pydivkit-29.9.0/pydivkit/div/div_disappear_action.py
+-rw-r--r--   0        0        0     1184 2024-03-11 13:52:24.288759 pydivkit-29.9.0/pydivkit/div/div_download_callbacks.py
+-rw-r--r--   0        0        0      302 2024-03-11 13:52:24.288935 pydivkit-29.9.0/pydivkit/div/div_drawable.py
+-rw-r--r--   0        0        0     2081 2024-03-11 13:52:24.293491 pydivkit-29.9.0/pydivkit/div/div_edge_insets.py
+-rw-r--r--   0        0        0      804 2024-03-11 13:52:24.291620 pydivkit-29.9.0/pydivkit/div/div_extension.py
+-rw-r--r--   0        0        0     1675 2024-03-11 13:52:24.296687 pydivkit-29.9.0/pydivkit/div/div_fade_transition.py
+-rw-r--r--   0        0        0      340 2024-03-11 13:52:24.293893 pydivkit-29.9.0/pydivkit/div/div_filter.py
+-rw-r--r--   0        0        0      564 2024-03-11 13:52:24.295831 pydivkit-29.9.0/pydivkit/div/div_filter_rtl_mirror.py
+-rw-r--r--   0        0        0      686 2024-03-11 13:52:24.299715 pydivkit-29.9.0/pydivkit/div/div_fixed_count.py
+-rw-r--r--   0        0        0     3267 2024-03-11 13:52:24.305275 pydivkit-29.9.0/pydivkit/div/div_fixed_length_input_mask.py
+-rw-r--r--   0        0        0     1090 2024-03-11 13:52:24.303838 pydivkit-29.9.0/pydivkit/div/div_fixed_size.py
+-rw-r--r--   0        0        0     2850 2024-03-11 13:52:24.304255 pydivkit-29.9.0/pydivkit/div/div_focus.py
+-rw-r--r--   0        0        0      300 2024-03-11 13:52:24.301469 pydivkit-29.9.0/pydivkit/div/div_font_weight.py
+-rw-r--r--   0        0        0    15161 2024-03-11 13:52:24.327998 pydivkit-29.9.0/pydivkit/div/div_gallery.py
+-rw-r--r--   0        0        0    14187 2024-03-11 13:52:24.330015 pydivkit-29.9.0/pydivkit/div/div_gif_image.py
+-rw-r--r--   0        0        0    12660 2024-03-11 13:52:24.329355 pydivkit-29.9.0/pydivkit/div/div_grid.py
+-rw-r--r--   0        0        0    15911 2024-03-11 13:52:24.337108 pydivkit-29.9.0/pydivkit/div/div_image.py
+-rw-r--r--   0        0        0     2530 2024-03-11 13:52:24.314267 pydivkit-29.9.0/pydivkit/div/div_image_background.py
+-rw-r--r--   0        0        0      300 2024-03-11 13:52:24.310451 pydivkit-29.9.0/pydivkit/div/div_image_scale.py
+-rw-r--r--   0        0        0    13843 2024-03-11 13:52:24.336847 pydivkit-29.9.0/pydivkit/div/div_indicator.py
+-rw-r--r--   0        0        0      490 2024-03-11 13:52:24.313107 pydivkit-29.9.0/pydivkit/div/div_indicator_item_placement.py
+-rw-r--r--   0        0        0      516 2024-03-11 13:52:24.316155 pydivkit-29.9.0/pydivkit/div/div_infinity_count.py
+-rw-r--r--   0        0        0    16238 2024-03-11 13:52:24.349718 pydivkit-29.9.0/pydivkit/div/div_input.py
+-rw-r--r--   0        0        0      478 2024-03-11 13:52:24.318154 pydivkit-29.9.0/pydivkit/div/div_input_mask.py
+-rw-r--r--   0        0        0      648 2024-03-11 13:52:24.320834 pydivkit-29.9.0/pydivkit/div/div_input_mask_base.py
+-rw-r--r--   0        0        0      424 2024-03-11 13:52:24.323139 pydivkit-29.9.0/pydivkit/div/div_input_validator.py
+-rw-r--r--   0        0        0     1277 2024-03-11 13:52:24.328285 pydivkit-29.9.0/pydivkit/div/div_input_validator_base.py
+-rw-r--r--   0        0        0     1719 2024-03-11 13:52:24.332768 pydivkit-29.9.0/pydivkit/div/div_input_validator_expression.py
+-rw-r--r--   0        0        0     1628 2024-03-11 13:52:24.336382 pydivkit-29.9.0/pydivkit/div/div_input_validator_regex.py
+-rw-r--r--   0        0        0      255 2024-03-11 13:52:24.334144 pydivkit-29.9.0/pydivkit/div/div_line_style.py
+-rw-r--r--   0        0        0     1046 2024-03-11 13:52:24.338070 pydivkit-29.9.0/pydivkit/div/div_linear_gradient.py
+-rw-r--r--   0        0        0      974 2024-03-11 13:52:24.337616 pydivkit-29.9.0/pydivkit/div/div_match_parent_size.py
+-rw-r--r--   0        0        0      858 2024-03-11 13:52:24.339147 pydivkit-29.9.0/pydivkit/div/div_neighbour_page_size.py
+-rw-r--r--   0        0        0     1297 2024-03-11 13:52:24.341486 pydivkit-29.9.0/pydivkit/div/div_nine_patch_background.py
+-rw-r--r--   0        0        0      795 2024-03-11 13:52:24.342771 pydivkit-29.9.0/pydivkit/div/div_page_size.py
+-rw-r--r--   0        0        0    13227 2024-03-11 13:52:24.364321 pydivkit-29.9.0/pydivkit/div/div_pager.py
+-rw-r--r--   0        0        0      369 2024-03-11 13:52:24.340734 pydivkit-29.9.0/pydivkit/div/div_pager_layout_mode.py
+-rw-r--r--   0        0        0     1928 2024-03-11 13:52:24.346710 pydivkit-29.9.0/pydivkit/div/div_patch.py
+-rw-r--r--   0        0        0      694 2024-03-11 13:52:24.344315 pydivkit-29.9.0/pydivkit/div/div_percentage_size.py
+-rw-r--r--   0        0        0      820 2024-03-11 13:52:24.345607 pydivkit-29.9.0/pydivkit/div/div_phone_input_mask.py
+-rw-r--r--   0        0        0      357 2024-03-11 13:52:24.345163 pydivkit-29.9.0/pydivkit/div/div_pivot.py
+-rw-r--r--   0        0        0     1136 2024-03-11 13:52:24.348597 pydivkit-29.9.0/pydivkit/div/div_pivot_fixed.py
+-rw-r--r--   0        0        0      800 2024-03-11 13:52:24.348963 pydivkit-29.9.0/pydivkit/div/div_pivot_percentage.py
+-rw-r--r--   0        0        0      768 2024-03-11 13:52:24.348878 pydivkit-29.9.0/pydivkit/div/div_point.py
+-rw-r--r--   0        0        0     1933 2024-03-11 13:52:24.353543 pydivkit-29.9.0/pydivkit/div/div_radial_gradient.py
+-rw-r--r--   0        0        0      473 2024-03-11 13:52:24.349467 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_center.py
+-rw-r--r--   0        0        0     1156 2024-03-11 13:52:24.353853 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_fixed_center.py
+-rw-r--r--   0        0        0      412 2024-03-11 13:52:24.352085 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_radius.py
+-rw-r--r--   0        0        0      800 2024-03-11 13:52:24.355691 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_center.py
+-rw-r--r--   0        0        0     1052 2024-03-11 13:52:24.357231 pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_radius.py
+-rw-r--r--   0        0        0     1721 2024-03-11 13:52:24.358941 pydivkit-29.9.0/pydivkit/div/div_rounded_rectangle_shape.py
+-rw-r--r--   0        0        0     2300 2024-03-11 13:52:24.360897 pydivkit-29.9.0/pydivkit/div/div_scale_transition.py
+-rw-r--r--   0        0        0    13666 2024-03-11 13:52:24.383982 pydivkit-29.9.0/pydivkit/div/div_select.py
+-rw-r--r--   0        0        0    12833 2024-03-11 13:52:24.381717 pydivkit-29.9.0/pydivkit/div/div_separator.py
+-rw-r--r--   0        0        0     1198 2024-03-11 13:52:24.360313 pydivkit-29.9.0/pydivkit/div/div_shadow.py
+-rw-r--r--   0        0        0      380 2024-03-11 13:52:24.360084 pydivkit-29.9.0/pydivkit/div/div_shape.py
+-rw-r--r--   0        0        0     1144 2024-03-11 13:52:24.365297 pydivkit-29.9.0/pydivkit/div/div_shape_drawable.py
+-rw-r--r--   0        0        0     2723 2024-03-11 13:52:24.366636 pydivkit-29.9.0/pydivkit/div/div_sight_action.py
+-rw-r--r--   0        0        0      424 2024-03-11 13:52:24.365181 pydivkit-29.9.0/pydivkit/div/div_size.py
+-rw-r--r--   0        0        0      256 2024-03-11 13:52:24.365974 pydivkit-29.9.0/pydivkit/div/div_size_unit.py
+-rw-r--r--   0        0        0     2360 2024-03-11 13:52:24.371447 pydivkit-29.9.0/pydivkit/div/div_slide_transition.py
+-rw-r--r--   0        0        0    16427 2024-03-11 13:52:24.399701 pydivkit-29.9.0/pydivkit/div/div_slider.py
+-rw-r--r--   0        0        0      700 2024-03-11 13:52:24.371633 pydivkit-29.9.0/pydivkit/div/div_solid_background.py
+-rw-r--r--   0        0        0    13669 2024-03-11 13:52:24.393749 pydivkit-29.9.0/pydivkit/div/div_state.py
+-rw-r--r--   0        0        0     1101 2024-03-11 13:52:24.372628 pydivkit-29.9.0/pydivkit/div/div_stretch_indicator_item_placement.py
+-rw-r--r--   0        0        0     1000 2024-03-11 13:52:24.374176 pydivkit-29.9.0/pydivkit/div/div_stroke.py
+-rw-r--r--   0        0        0    20352 2024-03-11 13:52:24.414134 pydivkit-29.9.0/pydivkit/div/div_tabs.py
+-rw-r--r--   0        0        0    25985 2024-03-11 13:52:24.463688 pydivkit-29.9.0/pydivkit/div/div_text.py
+-rw-r--r--   0        0        0      373 2024-03-11 13:52:24.376478 pydivkit-29.9.0/pydivkit/div/div_text_gradient.py
+-rw-r--r--   0        0        0      319 2024-03-11 13:52:24.379306 pydivkit-29.9.0/pydivkit/div/div_text_range_background.py
+-rw-r--r--   0        0        0      975 2024-03-11 13:52:24.382345 pydivkit-29.9.0/pydivkit/div/div_text_range_border.py
+-rw-r--r--   0        0        0     2706 2024-03-11 13:52:24.387093 pydivkit-29.9.0/pydivkit/div/div_timer.py
+-rw-r--r--   0        0        0     2922 2024-03-11 13:52:24.392564 pydivkit-29.9.0/pydivkit/div/div_tooltip.py
+-rw-r--r--   0        0        0     1171 2024-03-11 13:52:24.389188 pydivkit-29.9.0/pydivkit/div/div_transform.py
+-rw-r--r--   0        0        0     1234 2024-03-11 13:52:24.389715 pydivkit-29.9.0/pydivkit/div/div_transition_base.py
+-rw-r--r--   0        0        0      338 2024-03-11 13:52:24.393615 pydivkit-29.9.0/pydivkit/div/div_transition_selector.py
+-rw-r--r--   0        0        0      333 2024-03-11 13:52:24.394677 pydivkit-29.9.0/pydivkit/div/div_transition_trigger.py
+-rw-r--r--   0        0        0     1581 2024-03-11 13:52:24.398851 pydivkit-29.9.0/pydivkit/div/div_trigger.py
+-rw-r--r--   0        0        0      593 2024-03-11 13:52:24.396878 pydivkit-29.9.0/pydivkit/div/div_typed_value.py
+-rw-r--r--   0        0        0      663 2024-03-11 13:52:24.397628 pydivkit-29.9.0/pydivkit/div/div_variable.py
+-rw-r--r--   0        0        0    14446 2024-03-11 13:52:24.423923 pydivkit-29.9.0/pydivkit/div/div_video.py
+-rw-r--r--   0        0        0      276 2024-03-11 13:52:24.398912 pydivkit-29.9.0/pydivkit/div/div_video_scale.py
+-rw-r--r--   0        0        0     2331 2024-03-11 13:52:24.408006 pydivkit-29.9.0/pydivkit/div/div_video_source.py
+-rw-r--r--   0        0        0      286 2024-03-11 13:52:24.403528 pydivkit-29.9.0/pydivkit/div/div_visibility.py
+-rw-r--r--   0        0        0     3514 2024-03-11 13:52:24.407117 pydivkit-29.9.0/pydivkit/div/div_visibility_action.py
+-rw-r--r--   0        0        0     2298 2024-03-11 13:52:24.408418 pydivkit-29.9.0/pydivkit/div/div_wrap_content_size.py
+-rw-r--r--   0        0        0      611 2024-03-11 13:52:24.405665 pydivkit-29.9.0/pydivkit/div/integer_value.py
+-rw-r--r--   0        0        0      843 2024-03-11 13:52:24.410583 pydivkit-29.9.0/pydivkit/div/integer_variable.py
+-rw-r--r--   0        0        0      611 2024-03-11 13:52:24.411093 pydivkit-29.9.0/pydivkit/div/number_value.py
+-rw-r--r--   0        0        0      849 2024-03-11 13:52:24.414604 pydivkit-29.9.0/pydivkit/div/number_variable.py
+-rw-r--r--   0        0        0      607 2024-03-11 13:52:24.414132 pydivkit-29.9.0/pydivkit/div/string_value.py
+-rw-r--r--   0        0        0      837 2024-03-11 13:52:24.415706 pydivkit-29.9.0/pydivkit/div/string_variable.py
+-rw-r--r--   0        0        0      617 2024-03-11 13:52:24.416283 pydivkit-29.9.0/pydivkit/div/url_value.py
+-rw-r--r--   0        0        0      859 2024-03-11 13:52:24.417295 pydivkit-29.9.0/pydivkit/div/url_variable.py
+-rw-r--r--   0        0        0        0 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pydivkit/py.typed
+-rw-r--r--   0        0        0     1697 2024-03-11 13:51:44.836531 pydivkit-29.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-29.9.0/PKG-INFO
```

### Comparing `pydivkit-29.8.0/README.md` & `pydivkit-29.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/__init__.py` & `pydivkit-29.9.0/pydivkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/core/entities.py` & `pydivkit-29.9.0/pydivkit/core/entities.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/core/fields.py` & `pydivkit-29.9.0/pydivkit/core/fields.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/core/types/union.py` & `pydivkit-29.9.0/pydivkit/core/types/union.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/__init__.py` & `pydivkit-29.9.0/pydivkit/div/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/array_value.py` & `pydivkit-29.9.0/pydivkit/div/array_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/array_variable.py` & `pydivkit-29.9.0/pydivkit/div/array_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/boolean_value.py` & `pydivkit-29.9.0/pydivkit/div/boolean_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/boolean_variable.py` & `pydivkit-29.9.0/pydivkit/div/boolean_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/color_value.py` & `pydivkit-29.9.0/pydivkit/div/color_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/color_variable.py` & `pydivkit-29.9.0/pydivkit/div/color_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/content_text.py` & `pydivkit-29.9.0/pydivkit/div/content_text.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/content_url.py` & `pydivkit-29.9.0/pydivkit/div/content_url.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/dict_value.py` & `pydivkit-29.9.0/pydivkit/div/dict_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/dict_variable.py` & `pydivkit-29.9.0/pydivkit/div/dict_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div.py` & `pydivkit-29.9.0/pydivkit/div/div.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_absolute_edge_insets.py` & `pydivkit-29.9.0/pydivkit/div/div_absolute_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_accessibility.py` & `pydivkit-29.9.0/pydivkit/div/div_accessibility.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_action.py` & `pydivkit-29.9.0/pydivkit/div/div_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_action_array_insert_value.py` & `pydivkit-29.9.0/pydivkit/div/div_action_array_insert_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_action_array_remove_value.py` & `pydivkit-29.9.0/pydivkit/div/div_action_array_remove_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_action_copy_to_clipboard.py` & `pydivkit-29.9.0/pydivkit/div/div_action_copy_to_clipboard.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_action_focus_element.py` & `pydivkit-29.9.0/pydivkit/div/div_action_focus_element.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_action_set_variable.py` & `pydivkit-29.9.0/pydivkit/div/div_action_set_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_action_typed.py` & `pydivkit-29.9.0/pydivkit/div/div_action_typed.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_animation.py` & `pydivkit-29.9.0/pydivkit/div/div_animation.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_appearance_set_transition.py` & `pydivkit-29.9.0/pydivkit/div/div_appearance_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_appearance_transition.py` & `pydivkit-29.9.0/pydivkit/div/div_appearance_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_aspect.py` & `pydivkit-29.9.0/pydivkit/div/div_aspect.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_background.py` & `pydivkit-29.9.0/pydivkit/div/div_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_base.py` & `pydivkit-29.9.0/pydivkit/div/div_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_blur.py` & `pydivkit-29.9.0/pydivkit/div/div_blur.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_border.py` & `pydivkit-29.9.0/pydivkit/div/div_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_change_bounds_transition.py` & `pydivkit-29.9.0/pydivkit/div/div_change_bounds_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_change_set_transition.py` & `pydivkit-29.9.0/pydivkit/div/div_change_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_circle_shape.py` & `pydivkit-29.9.0/pydivkit/div/div_circle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_collection_item_builder.py` & `pydivkit-29.9.0/pydivkit/div/div_collection_item_builder.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_container.py` & `pydivkit-29.9.0/pydivkit/div/div_container.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_corners_radius.py` & `pydivkit-29.9.0/pydivkit/div/div_corners_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_currency_input_mask.py` & `pydivkit-29.9.0/pydivkit/div/div_currency_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_custom.py` & `pydivkit-29.9.0/pydivkit/div/div_custom.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_data.py` & `pydivkit-29.9.0/pydivkit/div/div_data.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_default_indicator_item_placement.py` & `pydivkit-29.9.0/pydivkit/div/div_default_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_dimension.py` & `pydivkit-29.9.0/pydivkit/div/div_dimension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_disappear_action.py` & `pydivkit-29.9.0/pydivkit/div/div_disappear_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_download_callbacks.py` & `pydivkit-29.9.0/pydivkit/div/div_download_callbacks.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_edge_insets.py` & `pydivkit-29.9.0/pydivkit/div/div_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_extension.py` & `pydivkit-29.9.0/pydivkit/div/div_extension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_fade_transition.py` & `pydivkit-29.9.0/pydivkit/div/div_fade_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_filter_rtl_mirror.py` & `pydivkit-29.9.0/pydivkit/div/div_filter_rtl_mirror.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_fixed_count.py` & `pydivkit-29.9.0/pydivkit/div/div_fixed_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_fixed_length_input_mask.py` & `pydivkit-29.9.0/pydivkit/div/div_fixed_length_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_fixed_size.py` & `pydivkit-29.9.0/pydivkit/div/div_fixed_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_focus.py` & `pydivkit-29.9.0/pydivkit/div/div_focus.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_gallery.py` & `pydivkit-29.9.0/pydivkit/div/div_gallery.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_gif_image.py` & `pydivkit-29.9.0/pydivkit/div/div_gif_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_grid.py` & `pydivkit-29.9.0/pydivkit/div/div_grid.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_image.py` & `pydivkit-29.9.0/pydivkit/div/div_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_image_background.py` & `pydivkit-29.9.0/pydivkit/div/div_image_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_indicator.py` & `pydivkit-29.9.0/pydivkit/div/div_indicator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_infinity_count.py` & `pydivkit-29.9.0/pydivkit/div/div_infinity_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_input.py` & `pydivkit-29.9.0/pydivkit/div/div_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,14 +340,15 @@
 class DivInputKeyboardType(str, enum.Enum):
     SINGLE_LINE_TEXT = "single_line_text"
     MULTI_LINE_TEXT = "multi_line_text"
     PHONE = "phone"
     NUMBER = "number"
     EMAIL = "email"
     URI = "uri"
+    PASSWORD = "password"
 
 
 # Text input line used in the native interface.
 class DivInputNativeInterface(BaseDiv):
 
     def __init__(
         self, *,
```

### Comparing `pydivkit-29.8.0/pydivkit/div/div_input_mask_base.py` & `pydivkit-29.9.0/pydivkit/div/div_input_mask_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_input_validator_base.py` & `pydivkit-29.9.0/pydivkit/div/div_input_validator_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_input_validator_expression.py` & `pydivkit-29.9.0/pydivkit/div/div_input_validator_expression.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_input_validator_regex.py` & `pydivkit-29.9.0/pydivkit/div/div_input_validator_regex.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_linear_gradient.py` & `pydivkit-29.9.0/pydivkit/div/div_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_match_parent_size.py` & `pydivkit-29.9.0/pydivkit/div/div_match_parent_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_neighbour_page_size.py` & `pydivkit-29.9.0/pydivkit/div/div_neighbour_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_nine_patch_background.py` & `pydivkit-29.9.0/pydivkit/div/div_nine_patch_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_page_size.py` & `pydivkit-29.9.0/pydivkit/div/div_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_pager.py` & `pydivkit-29.9.0/pydivkit/div/div_pager.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_patch.py` & `pydivkit-29.9.0/pydivkit/div/div_patch.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_percentage_size.py` & `pydivkit-29.9.0/pydivkit/div/div_percentage_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_phone_input_mask.py` & `pydivkit-29.9.0/pydivkit/div/div_phone_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_pivot_fixed.py` & `pydivkit-29.9.0/pydivkit/div/div_pivot_fixed.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_pivot_percentage.py` & `pydivkit-29.9.0/pydivkit/div/div_pivot_percentage.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_point.py` & `pydivkit-29.9.0/pydivkit/div/div_point.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_radial_gradient.py` & `pydivkit-29.9.0/pydivkit/div/div_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_radial_gradient_fixed_center.py` & `pydivkit-29.9.0/pydivkit/div/div_radial_gradient_fixed_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_radial_gradient_relative_center.py` & `pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_radial_gradient_relative_radius.py` & `pydivkit-29.9.0/pydivkit/div/div_radial_gradient_relative_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_rounded_rectangle_shape.py` & `pydivkit-29.9.0/pydivkit/div/div_rounded_rectangle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_scale_transition.py` & `pydivkit-29.9.0/pydivkit/div/div_scale_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_select.py` & `pydivkit-29.9.0/pydivkit/div/div_select.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_separator.py` & `pydivkit-29.9.0/pydivkit/div/div_separator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_shadow.py` & `pydivkit-29.9.0/pydivkit/div/div_shadow.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_shape_drawable.py` & `pydivkit-29.9.0/pydivkit/div/div_shape_drawable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_sight_action.py` & `pydivkit-29.9.0/pydivkit/div/div_sight_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_slide_transition.py` & `pydivkit-29.9.0/pydivkit/div/div_slide_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_slider.py` & `pydivkit-29.9.0/pydivkit/div/div_slider.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_solid_background.py` & `pydivkit-29.9.0/pydivkit/div/div_solid_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_state.py` & `pydivkit-29.9.0/pydivkit/div/div_state.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_stretch_indicator_item_placement.py` & `pydivkit-29.9.0/pydivkit/div/div_stretch_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_stroke.py` & `pydivkit-29.9.0/pydivkit/div/div_stroke.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_tabs.py` & `pydivkit-29.9.0/pydivkit/div/div_tabs.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_text.py` & `pydivkit-29.9.0/pydivkit/div/div_text.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_text_range_border.py` & `pydivkit-29.9.0/pydivkit/div/div_text_range_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_timer.py` & `pydivkit-29.9.0/pydivkit/div/div_timer.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_tooltip.py` & `pydivkit-29.9.0/pydivkit/div/div_tooltip.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_transform.py` & `pydivkit-29.9.0/pydivkit/div/div_transform.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_transition_base.py` & `pydivkit-29.9.0/pydivkit/div/div_transition_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_trigger.py` & `pydivkit-29.9.0/pydivkit/div/div_trigger.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_typed_value.py` & `pydivkit-29.9.0/pydivkit/div/div_typed_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_variable.py` & `pydivkit-29.9.0/pydivkit/div/div_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_video.py` & `pydivkit-29.9.0/pydivkit/div/div_video.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_video_source.py` & `pydivkit-29.9.0/pydivkit/div/div_video_source.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_visibility_action.py` & `pydivkit-29.9.0/pydivkit/div/div_visibility_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/div_wrap_content_size.py` & `pydivkit-29.9.0/pydivkit/div/div_wrap_content_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/integer_value.py` & `pydivkit-29.9.0/pydivkit/div/integer_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/integer_variable.py` & `pydivkit-29.9.0/pydivkit/div/integer_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/number_value.py` & `pydivkit-29.9.0/pydivkit/div/number_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/number_variable.py` & `pydivkit-29.9.0/pydivkit/div/number_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/string_value.py` & `pydivkit-29.9.0/pydivkit/div/string_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/string_variable.py` & `pydivkit-29.9.0/pydivkit/div/string_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/url_value.py` & `pydivkit-29.9.0/pydivkit/div/url_value.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pydivkit/div/url_variable.py` & `pydivkit-29.9.0/pydivkit/div/url_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-29.8.0/pyproject.toml` & `pydivkit-29.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydivkit"
-version = "29.8.0"
+version = "29.9.0"
 description = "DivKit python library"
 readme = "README.md"
 repository = "https://github.com/divkit/divkit/tree/main/json-builder/python"
 keywords = ["divkit", "sdk"]
 authors = [
     "Vladislav Bakaev <bakaev-vlad@yandex-team.ru>",
     "Pavel Mosein <p-mosein@yandex-team.ru>",
```

### Comparing `pydivkit-29.8.0/PKG-INFO` & `pydivkit-29.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydivkit
-Version: 29.8.0
+Version: 29.9.0
 Summary: DivKit python library
 Home-page: https://github.com/divkit/divkit/tree/main/json-builder/python
 Keywords: divkit,sdk
 Author: Vladislav Bakaev
 Author-email: bakaev-vlad@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

