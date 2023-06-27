# Comparing `tmp/pydivkit-13.0.0b0.tar.gz` & `tmp/pydivkit-25.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivkit-13.0.0b0.tar", max compression
+gzip compressed data, was "pydivkit-25.6.0.tar", max compression
```

## Comparing `pydivkit-13.0.0b0.tar` & `pydivkit-25.6.0.tar`

### file list

```diff
@@ -1,121 +1,128 @@
--rw-r--r--   0        0        0     9436 2022-10-27 11:17:29.614491 pydivkit-13.0.0b0/README.md
--rw-r--r--   0        0        0      689 2022-10-27 11:16:33.819102 pydivkit-13.0.0b0/pydivkit/__init__.py
--rw-r--r--   0        0        0      145 2022-10-27 11:16:33.819102 pydivkit-13.0.0b0/pydivkit/core/__init__.py
--rw-r--r--   0        0        0      395 2022-10-26 15:06:17.452227 pydivkit-13.0.0b0/pydivkit/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      322 2022-10-26 15:58:38.462641 pydivkit-13.0.0b0/pydivkit/core/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      957 2022-10-26 15:06:17.487896 pydivkit-13.0.0b0/pydivkit/core/__pycache__/compat.cpython-310.pyc
--rw-r--r--   0        0        0      956 2022-10-26 15:47:09.423069 pydivkit-13.0.0b0/pydivkit/core/__pycache__/compat.cpython-38.pyc
--rw-r--r--   0        0        0    21065 2022-10-26 15:06:17.461272 pydivkit-13.0.0b0/pydivkit/core/__pycache__/entities.cpython-310.pyc
--rw-r--r--   0        0        0    20571 2022-10-26 15:47:09.388105 pydivkit-13.0.0b0/pydivkit/core/__pycache__/entities.cpython-38.pyc
--rw-r--r--   0        0        0     2980 2022-10-26 08:40:16.019097 pydivkit-13.0.0b0/pydivkit/core/__pycache__/fields.cpython-310.pyc
--rw-r--r--   0        0        0     2775 2022-10-26 15:47:09.429689 pydivkit-13.0.0b0/pydivkit/core/__pycache__/fields.cpython-38.pyc
--rw-r--r--   0        0        0      445 2022-10-27 11:16:33.819102 pydivkit-13.0.0b0/pydivkit/core/compat.py
--rw-r--r--   0        0        0    26570 2022-10-27 11:16:33.819102 pydivkit-13.0.0b0/pydivkit/core/entities.py
--rw-r--r--   0        0        0     2667 2022-10-24 13:56:22.848462 pydivkit-13.0.0b0/pydivkit/core/fields.py
--rw-r--r--   0        0        0        0 2022-10-24 13:17:58.541756 pydivkit-13.0.0b0/pydivkit/core/types/__init__.py
--rw-r--r--   0        0        0      182 2022-10-26 08:40:16.025762 pydivkit-13.0.0b0/pydivkit/core/types/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      180 2022-10-26 15:47:09.442318 pydivkit-13.0.0b0/pydivkit/core/types/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      793 2022-10-26 08:40:16.026736 pydivkit-13.0.0b0/pydivkit/core/types/__pycache__/union.cpython-310.pyc
--rw-r--r--   0        0        0      785 2022-10-26 15:47:09.445699 pydivkit-13.0.0b0/pydivkit/core/types/__pycache__/union.cpython-38.pyc
--rw-r--r--   0        0        0      728 2022-10-24 13:17:58.541756 pydivkit-13.0.0b0/pydivkit/core/types/union.py
--rw-r--r--   0        0        0    10953 2022-10-27 12:09:17.052546 pydivkit-13.0.0b0/pydivkit/div/__init__.py
--rw-r--r--   0        0        0      698 2022-10-27 12:09:17.031265 pydivkit-13.0.0b0/pydivkit/div/boolean_variable.py
--rw-r--r--   0        0        0      712 2022-10-27 12:09:17.039812 pydivkit-13.0.0b0/pydivkit/div/color_variable.py
--rw-r--r--   0        0        0      784 2022-10-27 12:09:17.034084 pydivkit-13.0.0b0/pydivkit/div/div.py
--rw-r--r--   0        0        0     1004 2022-10-27 12:09:16.756736 pydivkit-13.0.0b0/pydivkit/div/div_absolute_edge_insets.py
--rw-r--r--   0        0        0     2882 2022-10-27 12:09:16.777513 pydivkit-13.0.0b0/pydivkit/div/div_accessibility.py
--rw-r--r--   0        0        0     3257 2022-10-27 12:09:16.775540 pydivkit-13.0.0b0/pydivkit/div/div_action.py
--rw-r--r--   0        0        0      279 2022-10-27 12:09:16.767159 pydivkit-13.0.0b0/pydivkit/div/div_alignment_horizontal.py
--rw-r--r--   0        0        0      303 2022-10-27 12:09:17.044006 pydivkit-13.0.0b0/pydivkit/div/div_alignment_vertical.py
--rw-r--r--   0        0        0     2708 2022-10-27 12:09:16.778060 pydivkit-13.0.0b0/pydivkit/div/div_animation.py
--rw-r--r--   0        0        0      365 2022-10-27 12:09:16.767172 pydivkit-13.0.0b0/pydivkit/div/div_animation_interpolator.py
--rw-r--r--   0        0        0      789 2022-10-27 12:09:16.776218 pydivkit-13.0.0b0/pydivkit/div/div_appearance_set_transition.py
--rw-r--r--   0        0        0      551 2022-10-27 12:09:16.756592 pydivkit-13.0.0b0/pydivkit/div/div_appearance_transition.py
--rw-r--r--   0        0        0      548 2022-10-27 12:09:16.777395 pydivkit-13.0.0b0/pydivkit/div/div_aspect.py
--rw-r--r--   0        0        0      593 2022-10-27 12:09:16.777746 pydivkit-13.0.0b0/pydivkit/div/div_background.py
--rw-r--r--   0        0        0     9074 2022-10-27 12:09:16.787891 pydivkit-13.0.0b0/pydivkit/div/div_base.py
--rw-r--r--   0        0        0      363 2022-10-27 12:09:16.780754 pydivkit-13.0.0b0/pydivkit/div/div_blend_mode.py
--rw-r--r--   0        0        0     1559 2022-10-27 12:09:16.791055 pydivkit-13.0.0b0/pydivkit/div/div_border.py
--rw-r--r--   0        0        0     1225 2022-10-27 12:09:16.802498 pydivkit-13.0.0b0/pydivkit/div/div_change_bounds_transition.py
--rw-r--r--   0        0        0      719 2022-10-27 12:09:16.802528 pydivkit-13.0.0b0/pydivkit/div/div_change_set_transition.py
--rw-r--r--   0        0        0      414 2022-10-27 12:09:16.788105 pydivkit-13.0.0b0/pydivkit/div/div_change_transition.py
--rw-r--r--   0        0        0      657 2022-10-27 12:09:16.802608 pydivkit-13.0.0b0/pydivkit/div/div_circle_shape.py
--rw-r--r--   0        0        0    15341 2022-10-27 12:09:16.820356 pydivkit-13.0.0b0/pydivkit/div/div_container.py
--rw-r--r--   0        0        0     1643 2022-10-27 12:09:16.810090 pydivkit-13.0.0b0/pydivkit/div/div_corners_radius.py
--rw-r--r--   0        0        0      345 2022-10-27 12:09:16.802580 pydivkit-13.0.0b0/pydivkit/div/div_count.py
--rw-r--r--   0        0        0     9921 2022-10-27 12:09:16.827567 pydivkit-13.0.0b0/pydivkit/div/div_custom.py
--rw-r--r--   0        0        0     2309 2022-10-27 12:09:16.820478 pydivkit-13.0.0b0/pydivkit/div/div_data.py
--rw-r--r--   0        0        0      640 2022-10-27 12:09:16.814011 pydivkit-13.0.0b0/pydivkit/div/div_dimension.py
--rw-r--r--   0        0        0     1154 2022-10-27 12:09:16.814162 pydivkit-13.0.0b0/pydivkit/div/div_download_callbacks.py
--rw-r--r--   0        0        0      296 2022-10-27 12:09:16.811880 pydivkit-13.0.0b0/pydivkit/div/div_drawable.py
--rw-r--r--   0        0        0     1127 2022-10-27 12:09:16.818871 pydivkit-13.0.0b0/pydivkit/div/div_edge_insets.py
--rw-r--r--   0        0        0      705 2022-10-27 12:09:16.824181 pydivkit-13.0.0b0/pydivkit/div/div_extension.py
--rw-r--r--   0        0        0     1457 2022-10-27 12:09:16.842599 pydivkit-13.0.0b0/pydivkit/div/div_fade_transition.py
--rw-r--r--   0        0        0      564 2022-10-27 12:09:16.845349 pydivkit-13.0.0b0/pydivkit/div/div_fixed_count.py
--rw-r--r--   0        0        0      928 2022-10-27 12:09:16.840426 pydivkit-13.0.0b0/pydivkit/div/div_fixed_size.py
--rw-r--r--   0        0        0     2691 2022-10-27 12:09:16.834299 pydivkit-13.0.0b0/pydivkit/div/div_focus.py
--rw-r--r--   0        0        0      252 2022-10-27 12:09:16.845183 pydivkit-13.0.0b0/pydivkit/div/div_font_family.py
--rw-r--r--   0        0        0      294 2022-10-27 12:09:16.846813 pydivkit-13.0.0b0/pydivkit/div/div_font_weight.py
--rw-r--r--   0        0        0    13459 2022-10-27 12:09:16.861132 pydivkit-13.0.0b0/pydivkit/div/div_gallery.py
--rw-r--r--   0        0        0    13119 2022-10-27 12:09:16.864471 pydivkit-13.0.0b0/pydivkit/div/div_gif_image.py
--rw-r--r--   0        0        0    11864 2022-10-27 12:09:16.875592 pydivkit-13.0.0b0/pydivkit/div/div_grid.py
--rw-r--r--   0        0        0    14475 2022-10-27 12:09:16.884887 pydivkit-13.0.0b0/pydivkit/div/div_image.py
--rw-r--r--   0        0        0     1953 2022-10-27 12:09:16.861642 pydivkit-13.0.0b0/pydivkit/div/div_image_background.py
--rw-r--r--   0        0        0      270 2022-10-27 12:09:16.861262 pydivkit-13.0.0b0/pydivkit/div/div_image_scale.py
--rw-r--r--   0        0        0    11329 2022-10-27 12:09:16.879616 pydivkit-13.0.0b0/pydivkit/div/div_indicator.py
--rw-r--r--   0        0        0      458 2022-10-27 12:09:16.866879 pydivkit-13.0.0b0/pydivkit/div/div_infinity_count.py
--rw-r--r--   0        0        0    13736 2022-10-27 12:09:16.895821 pydivkit-13.0.0b0/pydivkit/div/div_input.py
--rw-r--r--   0        0        0      249 2022-10-27 12:09:16.879616 pydivkit-13.0.0b0/pydivkit/div/div_line_style.py
--rw-r--r--   0        0        0      880 2022-10-27 12:09:16.884119 pydivkit-13.0.0b0/pydivkit/div/div_linear_gradient.py
--rw-r--r--   0        0        0      876 2022-10-27 12:09:16.884888 pydivkit-13.0.0b0/pydivkit/div/div_match_parent_size.py
--rw-r--r--   0        0        0      776 2022-10-27 12:09:16.889585 pydivkit-13.0.0b0/pydivkit/div/div_neighbour_page_size.py
--rw-r--r--   0        0        0     1148 2022-10-27 12:09:16.894650 pydivkit-13.0.0b0/pydivkit/div/div_nine_patch_background.py
--rw-r--r--   0        0        0      733 2022-10-27 12:09:16.896837 pydivkit-13.0.0b0/pydivkit/div/div_page_size.py
--rw-r--r--   0        0        0    12079 2022-10-27 12:09:16.914739 pydivkit-13.0.0b0/pydivkit/div/div_pager.py
--rw-r--r--   0        0        0      363 2022-10-27 12:09:16.892316 pydivkit-13.0.0b0/pydivkit/div/div_pager_layout_mode.py
--rw-r--r--   0        0        0     1696 2022-10-27 12:09:16.904646 pydivkit-13.0.0b0/pydivkit/div/div_patch.py
--rw-r--r--   0        0        0      592 2022-10-27 12:09:16.909669 pydivkit-13.0.0b0/pydivkit/div/div_percentage_size.py
--rw-r--r--   0        0        0      351 2022-10-27 12:09:16.909711 pydivkit-13.0.0b0/pydivkit/div/div_pivot.py
--rw-r--r--   0        0        0     1020 2022-10-27 12:09:16.909699 pydivkit-13.0.0b0/pydivkit/div/div_pivot_fixed.py
--rw-r--r--   0        0        0      667 2022-10-27 12:09:16.923144 pydivkit-13.0.0b0/pydivkit/div/div_pivot_percentage.py
--rw-r--r--   0        0        0      662 2022-10-27 12:09:16.912055 pydivkit-13.0.0b0/pydivkit/div/div_point.py
--rw-r--r--   0        0        0     1809 2022-10-27 12:09:16.940577 pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient.py
--rw-r--r--   0        0        0      467 2022-10-27 12:09:16.912060 pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient_center.py
--rw-r--r--   0        0        0     1013 2022-10-27 12:09:16.933098 pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient_fixed_center.py
--rw-r--r--   0        0        0      406 2022-10-27 12:09:16.921866 pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient_radius.py
--rw-r--r--   0        0        0      716 2022-10-27 12:09:16.933223 pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient_relative_center.py
--rw-r--r--   0        0        0      926 2022-10-27 12:09:16.940619 pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient_relative_radius.py
--rw-r--r--   0        0        0     1200 2022-10-27 12:09:16.945521 pydivkit-13.0.0b0/pydivkit/div/div_rounded_rectangle_shape.py
--rw-r--r--   0        0        0     2002 2022-10-27 12:09:16.953270 pydivkit-13.0.0b0/pydivkit/div/div_scale_transition.py
--rw-r--r--   0        0        0    12076 2022-10-27 12:09:16.966919 pydivkit-13.0.0b0/pydivkit/div/div_separator.py
--rw-r--r--   0        0        0      996 2022-10-27 12:09:16.944228 pydivkit-13.0.0b0/pydivkit/div/div_shadow.py
--rw-r--r--   0        0        0      374 2022-10-27 12:09:16.946474 pydivkit-13.0.0b0/pydivkit/div/div_shape.py
--rw-r--r--   0        0        0      974 2022-10-27 12:09:16.962613 pydivkit-13.0.0b0/pydivkit/div/div_shape_drawable.py
--rw-r--r--   0        0        0      418 2022-10-27 12:09:16.955583 pydivkit-13.0.0b0/pydivkit/div/div_size.py
--rw-r--r--   0        0        0      250 2022-10-27 12:09:16.966873 pydivkit-13.0.0b0/pydivkit/div/div_size_unit.py
--rw-r--r--   0        0        0     2142 2022-10-27 12:09:16.975787 pydivkit-13.0.0b0/pydivkit/div/div_slide_transition.py
--rw-r--r--   0        0        0    13771 2022-10-27 12:09:16.992015 pydivkit-13.0.0b0/pydivkit/div/div_slider.py
--rw-r--r--   0        0        0      578 2022-10-27 12:09:16.983927 pydivkit-13.0.0b0/pydivkit/div/div_solid_background.py
--rw-r--r--   0        0        0    12325 2022-10-27 12:09:17.000490 pydivkit-13.0.0b0/pydivkit/div/div_state.py
--rw-r--r--   0        0        0      798 2022-10-27 12:09:16.979080 pydivkit-13.0.0b0/pydivkit/div/div_stroke.py
--rw-r--r--   0        0        0    18824 2022-10-27 12:09:17.006415 pydivkit-13.0.0b0/pydivkit/div/div_tabs.py
--rw-r--r--   0        0        0    22723 2022-10-27 12:09:17.012369 pydivkit-13.0.0b0/pydivkit/div/div_text.py
--rw-r--r--   0        0        0      367 2022-10-27 12:09:16.978808 pydivkit-13.0.0b0/pydivkit/div/div_text_gradient.py
--rw-r--r--   0        0        0     2673 2022-10-27 12:09:16.997414 pydivkit-13.0.0b0/pydivkit/div/div_tooltip.py
--rw-r--r--   0        0        0     1111 2022-10-27 12:09:16.995727 pydivkit-13.0.0b0/pydivkit/div/div_transform.py
--rw-r--r--   0        0        0     1056 2022-10-27 12:09:16.998871 pydivkit-13.0.0b0/pydivkit/div/div_transition_base.py
--rw-r--r--   0        0        0      332 2022-10-27 12:09:17.002563 pydivkit-13.0.0b0/pydivkit/div/div_transition_selector.py
--rw-r--r--   0        0        0      327 2022-10-27 12:09:17.012890 pydivkit-13.0.0b0/pydivkit/div/div_transition_trigger.py
--rw-r--r--   0        0        0     1387 2022-10-27 12:09:17.019852 pydivkit-13.0.0b0/pydivkit/div/div_trigger.py
--rw-r--r--   0        0        0      560 2022-10-27 12:09:17.008264 pydivkit-13.0.0b0/pydivkit/div/div_variable.py
--rw-r--r--   0        0        0      280 2022-10-27 12:09:17.040465 pydivkit-13.0.0b0/pydivkit/div/div_visibility.py
--rw-r--r--   0        0        0     2634 2022-10-27 12:09:17.028348 pydivkit-13.0.0b0/pydivkit/div/div_visibility_action.py
--rw-r--r--   0        0        0      803 2022-10-27 12:09:17.042524 pydivkit-13.0.0b0/pydivkit/div/div_wrap_content_size.py
--rw-r--r--   0        0        0      680 2022-10-27 12:09:17.026878 pydivkit-13.0.0b0/pydivkit/div/integer_variable.py
--rw-r--r--   0        0        0      686 2022-10-27 12:09:17.020634 pydivkit-13.0.0b0/pydivkit/div/number_variable.py
--rw-r--r--   0        0        0      674 2022-10-27 12:09:17.021296 pydivkit-13.0.0b0/pydivkit/div/string_variable.py
--rw-r--r--   0        0        0      696 2022-10-27 12:09:17.040005 pydivkit-13.0.0b0/pydivkit/div/url_variable.py
--rw-r--r--   0        0        0        0 2022-10-27 11:16:33.799575 pydivkit-13.0.0b0/pydivkit/py.typed
--rw-r--r--   0        0        0     1732 2022-10-27 12:23:50.524314 pydivkit-13.0.0b0/pyproject.toml
--rw-r--r--   0        0        0    10499 2022-10-27 12:23:55.185794 pydivkit-13.0.0b0/setup.py
--rw-r--r--   0        0        0    10826 2022-10-27 12:23:55.186215 pydivkit-13.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     9446 2023-06-27 11:05:18.333821 pydivkit-25.6.0/README.md
+-rw-r--r--   0        0        0      700 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/compat.py
+-rw-r--r--   0        0        0    28631 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/entities.py
+-rw-r--r--   0        0        0     3039 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/fields.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/types/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/types/union.py
+-rw-r--r--   0        0        0    13558 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/__init__.py
+-rw-r--r--   0        0        0      884 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/boolean_variable.py
+-rw-r--r--   0        0        0      898 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/color_variable.py
+-rw-r--r--   0        0        0      863 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div.py
+-rw-r--r--   0        0        0     1209 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_absolute_edge_insets.py
+-rw-r--r--   0        0        0     3263 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_accessibility.py
+-rw-r--r--   0        0        0     3671 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_action.py
+-rw-r--r--   0        0        0      285 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_alignment_horizontal.py
+-rw-r--r--   0        0        0      309 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_alignment_vertical.py
+-rw-r--r--   0        0        0     3038 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_animation.py
+-rw-r--r--   0        0        0      371 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_animation_interpolator.py
+-rw-r--r--   0        0        0      879 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_appearance_set_transition.py
+-rw-r--r--   0        0        0      557 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_appearance_transition.py
+-rw-r--r--   0        0        0      671 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_aspect.py
+-rw-r--r--   0        0        0      599 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_background.py
+-rw-r--r--   0        0        0     9833 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_base.py
+-rw-r--r--   0        0        0      369 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_blend_mode.py
+-rw-r--r--   0        0        0      764 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_blur.py
+-rw-r--r--   0        0        0     1697 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_border.py
+-rw-r--r--   0        0        0     1403 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_change_bounds_transition.py
+-rw-r--r--   0        0        0      809 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_change_set_transition.py
+-rw-r--r--   0        0        0      420 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_change_transition.py
+-rw-r--r--   0        0        0     1176 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_circle_shape.py
+-rw-r--r--   0        0        0    17322 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_container.py
+-rw-r--r--   0        0        0     1861 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_corners_radius.py
+-rw-r--r--   0        0        0      351 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_count.py
+-rw-r--r--   0        0        0     1292 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_currency_input_mask.py
+-rw-r--r--   0        0        0    10752 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_custom.py
+-rw-r--r--   0        0        0     2915 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_data.py
+-rw-r--r--   0        0        0      872 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_default_indicator_item_placement.py
+-rw-r--r--   0        0        0      802 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_dimension.py
+-rw-r--r--   0        0        0     2952 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_disappear_action.py
+-rw-r--r--   0        0        0     1228 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_download_callbacks.py
+-rw-r--r--   0        0        0      302 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_drawable.py
+-rw-r--r--   0        0        0     1385 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_edge_insets.py
+-rw-r--r--   0        0        0      827 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_extension.py
+-rw-r--r--   0        0        0     1675 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fade_transition.py
+-rw-r--r--   0        0        0      271 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_filter.py
+-rw-r--r--   0        0        0      686 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fixed_count.py
+-rw-r--r--   0        0        0     3313 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fixed_length_input_mask.py
+-rw-r--r--   0        0        0     1090 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fixed_size.py
+-rw-r--r--   0        0        0     3026 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_focus.py
+-rw-r--r--   0        0        0      258 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_font_family.py
+-rw-r--r--   0        0        0      300 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_font_weight.py
+-rw-r--r--   0        0        0    14582 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_gallery.py
+-rw-r--r--   0        0        0    14431 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_gif_image.py
+-rw-r--r--   0        0        0    12886 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_grid.py
+-rw-r--r--   0        0        0    16177 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_image.py
+-rw-r--r--   0        0        0     2552 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_image_background.py
+-rw-r--r--   0        0        0      300 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_image_scale.py
+-rw-r--r--   0        0        0    13998 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_indicator.py
+-rw-r--r--   0        0        0      490 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_indicator_item_placement.py
+-rw-r--r--   0        0        0      516 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_infinity_count.py
+-rw-r--r--   0        0        0    15687 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input.py
+-rw-r--r--   0        0        0      403 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_mask.py
+-rw-r--r--   0        0        0      671 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_mask_base.py
+-rw-r--r--   0        0        0      424 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator.py
+-rw-r--r--   0        0        0     1249 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator_base.py
+-rw-r--r--   0        0        0     1590 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator_expression.py
+-rw-r--r--   0        0        0     1548 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator_regex.py
+-rw-r--r--   0        0        0      255 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_line_style.py
+-rw-r--r--   0        0        0     1046 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_linear_gradient.py
+-rw-r--r--   0        0        0      974 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_match_parent_size.py
+-rw-r--r--   0        0        0      858 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_neighbour_page_size.py
+-rw-r--r--   0        0        0     1297 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_nine_patch_background.py
+-rw-r--r--   0        0        0      795 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_page_size.py
+-rw-r--r--   0        0        0    13014 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pager.py
+-rw-r--r--   0        0        0      369 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pager_layout_mode.py
+-rw-r--r--   0        0        0     1950 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_patch.py
+-rw-r--r--   0        0        0      694 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_percentage_size.py
+-rw-r--r--   0        0        0      357 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pivot.py
+-rw-r--r--   0        0        0     1136 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pivot_fixed.py
+-rw-r--r--   0        0        0      800 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pivot_percentage.py
+-rw-r--r--   0        0        0      768 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_point.py
+-rw-r--r--   0        0        0     1933 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient.py
+-rw-r--r--   0        0        0      473 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_center.py
+-rw-r--r--   0        0        0     1156 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_fixed_center.py
+-rw-r--r--   0        0        0      412 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_radius.py
+-rw-r--r--   0        0        0      800 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_relative_center.py
+-rw-r--r--   0        0        0     1052 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_relative_radius.py
+-rw-r--r--   0        0        0     1721 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_rounded_rectangle_shape.py
+-rw-r--r--   0        0        0     2300 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_scale_transition.py
+-rw-r--r--   0        0        0    13936 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_select.py
+-rw-r--r--   0        0        0    13054 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_separator.py
+-rw-r--r--   0        0        0     1198 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_shadow.py
+-rw-r--r--   0        0        0      380 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_shape.py
+-rw-r--r--   0        0        0     1144 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_shape_drawable.py
+-rw-r--r--   0        0        0      424 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_size.py
+-rw-r--r--   0        0        0      256 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_size_unit.py
+-rw-r--r--   0        0        0     2360 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_slide_transition.py
+-rw-r--r--   0        0        0    15030 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_slider.py
+-rw-r--r--   0        0        0      700 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_solid_background.py
+-rw-r--r--   0        0        0    13360 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_state.py
+-rw-r--r--   0        0        0     1101 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_stretch_indicator_item_placement.py
+-rw-r--r--   0        0        0     1000 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_stroke.py
+-rw-r--r--   0        0        0    20599 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_tabs.py
+-rw-r--r--   0        0        0    25719 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text.py
+-rw-r--r--   0        0        0      373 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text_gradient.py
+-rw-r--r--   0        0        0      319 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text_range_background.py
+-rw-r--r--   0        0        0      975 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text_range_border.py
+-rw-r--r--   0        0        0     2796 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_timer.py
+-rw-r--r--   0        0        0     2923 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_tooltip.py
+-rw-r--r--   0        0        0     1171 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transform.py
+-rw-r--r--   0        0        0     1234 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transition_base.py
+-rw-r--r--   0        0        0      338 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transition_selector.py
+-rw-r--r--   0        0        0      333 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transition_trigger.py
+-rw-r--r--   0        0        0     1581 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_trigger.py
+-rw-r--r--   0        0        0      566 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_variable.py
+-rw-r--r--   0        0        0    13711 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_video.py
+-rw-r--r--   0        0        0     2826 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_video_source.py
+-rw-r--r--   0        0        0      286 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_visibility.py
+-rw-r--r--   0        0        0     2956 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_visibility_action.py
+-rw-r--r--   0        0        0     2298 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_wrap_content_size.py
+-rw-r--r--   0        0        0      866 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/integer_variable.py
+-rw-r--r--   0        0        0      872 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/number_variable.py
+-rw-r--r--   0        0        0      860 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/string_variable.py
+-rw-r--r--   0        0        0      882 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/url_variable.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/py.typed
+-rw-r--r--   0        0        0     1697 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-25.6.0/PKG-INFO
```

### Comparing `pydivkit-13.0.0b0/README.md` & `pydivkit-25.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 PyDIVKit examples
 =================
 
-This library is for working with DivKit with python.
+This library is designed to work with [DivKit](http://divkit.tech/) with python.
 
 Features:
 * Declarative and imperative DivKit blocks definition
 * Native Type-hints support
 * Complete object-oriented API
 * IDE type checks and suggestions
 
 Object construction
 -------------------
 
-The main idea is a provides ability to construct blocks by python objects.
+The main idea is to provide a tool for creating blocks using Python objects.
 
 ```python
 import json
 import pydivkit as dk
 
 container = dk.DivContainer(
     items=[
@@ -162,17 +162,17 @@
 #  ]
 # }
 ```
 
 Templating and DRY
 ------------------
 
-Of course building blocks from your code every time manually it's
-a very boring. So the first idea it's a move initialization of the 
-DivKit objects to the functions.
+Of course, manually building blocks from your code every time is boring. 
+So, the first idea is to move the initialization of DivKit objects 
+into functions.
 
 ```python
 # Naive DRY example which strictly non-recommended
 import pydivkit as dk
 
 
 def get_size(value: int = 32) -> dk.DivFixedSize:
@@ -209,15 +209,15 @@
 Looks a little better, but this approach doesn't scale well. To simplify layout 
 and save traffic, DivKit has templates. This is a way to layout similar elements
 without having to declare the complete json, but just declare a template and use
 this many times in similar items.
 
 **PyDivKit supports defining templates through the inheritance.**
 
-Let's define an example card.
+Let's define an example card:
 
 ```python
 import json
 
 import pydivkit as dk
 
 
@@ -362,16 +362,16 @@
 Template names
 --------------
 
 By default, templates are collecting by the metaclass into shared storage when 
 the class is declaring at import time, and have the 
 format `{module_name}.{class_name}`.
 
-The following example, which I am sure will not occur in the wild, shows a 
-warning if suddenly the names of the classes, and hence the templates, conflict.
+The following example, sure will not occur in the wild, shows a warning if 
+suddenly the names of the classes, and hence the templates, conflict.
 
 ```python
 import pydivkit as dk
 
 
 class MyTemplate(dk.DivContainer):
     width = dk.DivWrapContentSize()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/__init__.py` & `pydivkit-25.6.0/pydivkit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # flake8: noqa: F405
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pydivkit.core import Field, Ref
 from pydivkit.div import *
 from pydivkit.div import __all__ as __div_all__
 
 
-def make_card(log_id: str, *divs: Div):
+def make_card(log_id: str, *divs: Div) -> DivData:
     return DivData(
         log_id=log_id,
         states=[
             DivDataState(state_id=state_id, div=div)
             for state_id, div in enumerate(divs)
         ],
     )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/core/entities.py` & `pydivkit-25.6.0/pydivkit/core/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import uuid
 import warnings
 from collections import defaultdict
 from functools import reduce
 from types import MappingProxyType
 from typing import (
     Any, Dict, FrozenSet, List, Mapping, Optional, Sequence, Set, Type, Union,
-    get_args, get_origin, get_type_hints,
+    get_args, get_origin, get_type_hints, Iterator, Tuple,
 )
 
 from .compat import classproperty
-from .fields import _Field
+from .fields import Expr, _Field
 from .types.union import inject_types
 
 
 TYPE_FIELD = "type"
 
 # ExcludeFieldsType: str -> ExcludeFieldsType | bool
 ExcludeFieldsType = Mapping[str, Any]
@@ -50,24 +50,28 @@
     if isinstance(value, _Field):
         raise ValueError("Value cannot be of type _Field")
 
     if type_ is Any:
         return value
 
     origin_type = get_origin(type_)
-    if origin_type is list:
-        if not isinstance(value, list):
+
+    if isinstance(origin_type, type) and isinstance(origin_type, (str, bytes)):
+        return type_(value)
+
+    if isinstance(origin_type, type) and issubclass(origin_type, Sequence):
+        if not isinstance(value, Sequence):
             raise ValueError(
                 f"Value {value} has wrong type. Expected type is {type_}.",
             )
         element_type, *_ = get_args(type_)
         return [_cast_value_type(v, element_type) for v in value]
 
-    if origin_type is dict:
-        if not isinstance(value, dict):
+    if isinstance(origin_type, type) and issubclass(origin_type, Mapping):
+        if not isinstance(value, Mapping):
             raise ValueError(
                 f"Value {value} has wrong type. Expected type is {type_}.",
             )
 
         key_type, value_type = get_args(type_)
         return {
             _cast_value_type(k, key_type): _cast_value_type(v, value_type)
@@ -84,15 +88,17 @@
             if type_value:
                 target_type = types.get(type_value)
                 if target_type:
                     return target_type(**value)
                 raise ValueError(
                     f"Union {type_} does not contain type {type_value}.",
                 )
-            raise ValueError(f"Value {value} does not have field {TYPE_FIELD}.")
+            raise ValueError(
+                f"Value {value} does not have field {TYPE_FIELD}.",
+            )
         for u_type in get_args(type_):
             try:
                 return _cast_value_type(value, u_type)
             except ValueError:
                 pass
         raise ValueError(
             f"Value {value} has wrong type. Expected type is {type_}.",
@@ -119,19 +125,25 @@
 
     raise ValueError(
         f"Value {value} has wrong type. Expected type is {type_}.",
     )
 
 
 def dump(obj: Any) -> Any:
-    if isinstance(obj, list):
+    if isinstance(obj, (str, bytes)):
+        return obj
+    if isinstance(obj, Sequence):
         return [dump(obj_item) for obj_item in obj]
-    elif isinstance(obj, BaseEntity):
+    if isinstance(obj, Mapping):
+        return {k: v for k, v in obj.items()}
+    if isinstance(obj, Expr):
+        return str(obj)
+    if isinstance(obj, BaseEntity):
         return obj.dict()
-    elif isinstance(obj, enum.Enum):
+    if isinstance(obj, enum.Enum):
         return obj.value
     return obj
 
 
 def _update_related_templates(
     value: Any,
     related_templates: Set[Type[BaseDiv]],
@@ -169,14 +181,16 @@
             {
                 "type": "integer",
                 "enum": [0, 1],
                 "format": "boolean",
             },
         ),
         str: MappingProxyType({"type": "string"}),
+        bytes: MappingProxyType({"type": "string"}),
+        Expr: MappingProxyType({"type": "string", "pattern": "^@{.*}$"}),
     },
 )
 
 
 def _type_field_to_schema(field: _Field) -> SchemaType:
     return {
         "type": "string",
@@ -240,22 +254,22 @@
 ) -> SchemaType:
     type_ = _unpack_optional_type(type_)
     origin = get_origin(type_)
 
     schema: Optional[SchemaType] = None
     if field and field.name == TYPE_FIELD and field.default:
         schema = _type_field_to_schema(field)
-    elif origin is list:
+    elif type_ in BUILTIN_TYPES_TO_SCHEMA:
+        schema = {**BUILTIN_TYPES_TO_SCHEMA[type_]}
+    elif isinstance(origin, type) and issubclass(origin, Sequence):
         schema = _list_to_schema(type_, definitions, exclude)
-    elif origin is dict:
+    elif isinstance(origin, type) and issubclass(origin, Mapping):
         schema = _dict_to_schema()
     elif origin is Union:
         schema = _union_to_schema(field, type_, exclude, definitions)
-    elif type_ in BUILTIN_TYPES_TO_SCHEMA:
-        schema = {**BUILTIN_TYPES_TO_SCHEMA[type_]}
     elif issubclass(type_, BaseEntity):
         schema = type_.schema_as_ref(definitions, exclude)
     elif issubclass(type_, enum.Enum):
         schema = _enum_to_schema(type_)
 
     if not schema:
         raise TypeError(f"Schema building error for unknown type {type_}")
@@ -505,15 +519,17 @@
 
     def dict(self) -> Dict[str, Any]:
         result: Dict[str, Any] = {}
         for field_name, field in self.__fields__.items():
             field_value = getattr(self, field_name, field.default)
             if field_value is not None:
                 if isinstance(field_value, _Field) and field_value.ref_to:
-                    result[f"${field.field_name}"] = field_value.ref_to.field_name
+                    result[
+                        f"${field.field_name}"
+                    ] = field_value.ref_to.field_name
                 else:
                     result[field.field_name] = dump(field_value)
         return result
 
     @classmethod
     def _can_add_field_to_schema(
         cls,
@@ -677,26 +693,67 @@
                     ref_types[ref_uid],
                     field_type,
                 )
             else:
                 ref_types[ref_uid] = field_type
         return MappingProxyType(ref_types)
 
+    @staticmethod
+    def _make_union(type: Type[Any]) -> Set[Type[Any]]:
+        if get_origin(type) is Union:
+            return set(get_args(type))
+        return {type}
+
+    @classmethod
+    def _validate_subclass(
+        cls,
+        ref_type: Type[Any],
+        expected_field_type: Type[Any],
+    ) -> bool:
+        def _check_origins() -> Iterator[Tuple[Tuple[Any, ...], Tuple[Any, ...]]]:
+            for ref in cls._make_union(ref_type):
+                for expect in cls._make_union(expected_field_type):
+                    if get_origin(expect) == get_origin(ref):
+                        yield get_args(ref), get_args(expect)
+            return None
+
+        for origins in _check_origins():
+            if origins is None:
+                return False
+
+            expect, ref = origins
+
+            if get_args(expect) == get_args(ref):
+                return True
+
+            if not any(
+                issubclass(exp, get_args(ref))
+                for exp in get_args(expect)
+                if get_origin(exp) is not Union
+            ):
+                continue
+
+            return True
+        return False
+
     @classmethod
     def _validate_ref_types(cls) -> None:
         ref_types = cls._merge_ref_types(
             cls._extract_ref_types_from_fields(),
             cls._extract_ref_types_from_tpl_values(),
         )
         for ref_uid, ref_type in ref_types.items():
             field_name = cls.__field_names__[ref_uid]
             expected_field_type = cls.__field_types__[field_name]
             if (
                 ref_type != expected_field_type
                 and ref_type != Optional[expected_field_type]
+                and ref_type != Union[expected_field_type, Expr]
+                and ref_type != Union[expected_field_type, Expr, None]
+                and not cls._validate_subclass(ref_type, expected_field_type)
             ):
                 raise TypeError(
                     f"Type of attribute '{field_name}' does "
                     f"not match ref type {expected_field_type} != {ref_type}",
                 )
 
     @classmethod
```

### Comparing `pydivkit-13.0.0b0/pydivkit/core/fields.py` & `pydivkit-25.6.0/pydivkit/core/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     def field_name(self) -> str:
         if not self.name:
             raise ValueError("Field 'name' not initialized")
         return self.name
 
     def apply_constraints(self, constraints: Mapping[str, Any]) -> None:
         for c_key, c_value in constraints.items():
-            if self.constraints.get(c_key) and self.constraints[c_key] != c_value:
+            if self.constraints.get(c_key) and self.constraints[
+                c_key
+            ] != c_value:
                 raise ValueError(
                     f"Incompatible constraints: {c_key} = "
                     f"{self.constraints[c_key]} and {c_key} = {c_value}",
                 )
             self.constraints[c_key] = c_value
 
 
@@ -78,7 +80,23 @@
 def Ref(field: Any) -> Any:
     if not isinstance(field, _Field):
         raise ValueError(
             f"Value {field} has wrong type. Expected type is Field.",
         )
     field.is_ref = True
     return _Field(ref_to=field)
+
+
+class Expr:
+    __slots__ = ("v",)
+    v: str
+
+    def __init__(self, v: str):
+        if not v.startswith("@{") or not v.endswith("}"):
+            raise ValueError(f"failed to initiate Expr with {v}")
+        self.v = v
+
+    def __repr__(self) -> str:
+        return f"Expr({self.v})"
+
+    def __str__(self) -> str:
+        return self.v
```

### Comparing `pydivkit-13.0.0b0/pydivkit/core/types/union.py` & `pydivkit-25.6.0/pydivkit/core/types/union.py`

 * *Files identical despite different names*

### Comparing `pydivkit-13.0.0b0/pydivkit/div/__init__.py` & `pydivkit-25.6.0/pydivkit/div/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,50 +15,67 @@
 from .div_animation_interpolator import DivAnimationInterpolator
 from .div_appearance_set_transition import DivAppearanceSetTransition
 from .div_appearance_transition import DivAppearanceTransition
 from .div_aspect import DivAspect
 from .div_background import DivBackground
 from .div_base import DivBase
 from .div_blend_mode import DivBlendMode
+from .div_blur import DivBlur
 from .div_border import DivBorder
 from .div_change_bounds_transition import DivChangeBoundsTransition
 from .div_change_set_transition import DivChangeSetTransition
 from .div_change_transition import DivChangeTransition
 from .div_circle_shape import DivCircleShape
 from .div_container import (
     DivContainer, DivContainerLayoutMode, DivContainerOrientation,
     DivContainerSeparator,
 )
 from .div_corners_radius import DivCornersRadius
 from .div_count import DivCount
+from .div_currency_input_mask import DivCurrencyInputMask
 from .div_custom import DivCustom
 from .div_data import DivData, DivDataState
+from .div_default_indicator_item_placement import (
+    DivDefaultIndicatorItemPlacement,
+)
 from .div_dimension import DivDimension
+from .div_disappear_action import DivDisappearAction
 from .div_download_callbacks import DivDownloadCallbacks
 from .div_drawable import DivDrawable
 from .div_edge_insets import DivEdgeInsets
 from .div_extension import DivExtension
 from .div_fade_transition import DivFadeTransition
+from .div_filter import DivFilter
 from .div_fixed_count import DivFixedCount
+from .div_fixed_length_input_mask import (
+    DivFixedLengthInputMask, DivFixedLengthInputMaskPatternElement,
+)
 from .div_fixed_size import DivFixedSize
 from .div_focus import DivFocus, DivFocusNextFocusIds
 from .div_font_family import DivFontFamily
 from .div_font_weight import DivFontWeight
 from .div_gallery import (
     DivGallery, DivGalleryCrossContentAlignment, DivGalleryOrientation,
     DivGalleryScrollMode,
 )
 from .div_gif_image import DivGifImage
 from .div_grid import DivGrid
 from .div_image import DivImage
 from .div_image_background import DivImageBackground
 from .div_image_scale import DivImageScale
 from .div_indicator import DivIndicator, DivIndicatorAnimation
+from .div_indicator_item_placement import DivIndicatorItemPlacement
 from .div_infinity_count import DivInfinityCount
 from .div_input import DivInput, DivInputKeyboardType, DivInputNativeInterface
+from .div_input_mask import DivInputMask
+from .div_input_mask_base import DivInputMaskBase
+from .div_input_validator import DivInputValidator
+from .div_input_validator_base import DivInputValidatorBase
+from .div_input_validator_expression import DivInputValidatorExpression
+from .div_input_validator_regex import DivInputValidatorRegex
 from .div_line_style import DivLineStyle
 from .div_linear_gradient import DivLinearGradient
 from .div_match_parent_size import DivMatchParentSize
 from .div_neighbour_page_size import DivNeighbourPageSize
 from .div_nine_patch_background import DivNinePatchBackground
 from .div_page_size import DivPageSize
 from .div_pager import DivPager, DivPagerOrientation
@@ -75,44 +92,55 @@
 from .div_radial_gradient_radius import DivRadialGradientRadius
 from .div_radial_gradient_relative_center import DivRadialGradientRelativeCenter
 from .div_radial_gradient_relative_radius import (
     DivRadialGradientRelativeRadius, DivRadialGradientRelativeRadiusValue,
 )
 from .div_rounded_rectangle_shape import DivRoundedRectangleShape
 from .div_scale_transition import DivScaleTransition
+from .div_select import DivSelect, DivSelectOption
 from .div_separator import (
     DelimiterStyleOrientation, DivSeparator, DivSeparatorDelimiterStyle,
 )
 from .div_shadow import DivShadow
 from .div_shape import DivShape
 from .div_shape_drawable import DivShapeDrawable
 from .div_size import DivSize
 from .div_size_unit import DivSizeUnit
 from .div_slide_transition import DivSlideTransition, DivSlideTransitionEdge
 from .div_slider import DivSlider, DivSliderTextStyle
 from .div_solid_background import DivSolidBackground
 from .div_state import DivState, DivStateState
+from .div_stretch_indicator_item_placement import (
+    DivStretchIndicatorItemPlacement,
+)
 from .div_stroke import DivStroke
 from .div_tabs import (
     DivTabs, DivTabsItem, DivTabsTabTitleStyle, TabTitleStyleAnimationType,
 )
 from .div_text import (
     DivText, DivTextEllipsis, DivTextImage, DivTextRange, DivTextTruncate,
 )
 from .div_text_gradient import DivTextGradient
+from .div_text_range_background import DivTextRangeBackground
+from .div_text_range_border import DivTextRangeBorder
+from .div_timer import DivTimer
 from .div_tooltip import DivTooltip, DivTooltipPosition
 from .div_transform import DivTransform
 from .div_transition_base import DivTransitionBase
 from .div_transition_selector import DivTransitionSelector
 from .div_transition_trigger import DivTransitionTrigger
 from .div_trigger import DivTrigger, DivTriggerMode
 from .div_variable import DivVariable
+from .div_video import DivVideo
+from .div_video_source import DivVideoSource, DivVideoSourceResolution
 from .div_visibility import DivVisibility
 from .div_visibility_action import DivVisibilityAction
-from .div_wrap_content_size import DivWrapContentSize
+from .div_wrap_content_size import (
+    DivWrapContentSize, DivWrapContentSizeConstraintSize,
+)
 from .integer_variable import IntegerVariable
 from .number_variable import NumberVariable
 from .string_variable import StringVariable
 from .url_variable import UrlVariable
 
 
 BooleanVariable.update_forward_refs()
@@ -121,42 +149,52 @@
 DivAccessibility.update_forward_refs()
 DivAction.update_forward_refs()
 DivActionMenuItem.update_forward_refs()
 DivAnimation.update_forward_refs()
 DivAppearanceSetTransition.update_forward_refs()
 DivAspect.update_forward_refs()
 DivBase.update_forward_refs()
+DivBlur.update_forward_refs()
 DivBorder.update_forward_refs()
 DivChangeBoundsTransition.update_forward_refs()
 DivChangeSetTransition.update_forward_refs()
 DivCircleShape.update_forward_refs()
 DivContainer.update_forward_refs()
 DivContainerSeparator.update_forward_refs()
 DivCornersRadius.update_forward_refs()
+DivCurrencyInputMask.update_forward_refs()
 DivCustom.update_forward_refs()
 DivData.update_forward_refs()
 DivDataState.update_forward_refs()
+DivDefaultIndicatorItemPlacement.update_forward_refs()
 DivDimension.update_forward_refs()
+DivDisappearAction.update_forward_refs()
 DivDownloadCallbacks.update_forward_refs()
 DivEdgeInsets.update_forward_refs()
 DivExtension.update_forward_refs()
 DivFadeTransition.update_forward_refs()
 DivFixedCount.update_forward_refs()
+DivFixedLengthInputMask.update_forward_refs()
+DivFixedLengthInputMaskPatternElement.update_forward_refs()
 DivFixedSize.update_forward_refs()
 DivFocus.update_forward_refs()
 DivFocusNextFocusIds.update_forward_refs()
 DivGallery.update_forward_refs()
 DivGifImage.update_forward_refs()
 DivGrid.update_forward_refs()
 DivImage.update_forward_refs()
 DivImageBackground.update_forward_refs()
 DivIndicator.update_forward_refs()
 DivInfinityCount.update_forward_refs()
 DivInput.update_forward_refs()
 DivInputNativeInterface.update_forward_refs()
+DivInputMaskBase.update_forward_refs()
+DivInputValidatorBase.update_forward_refs()
+DivInputValidatorExpression.update_forward_refs()
+DivInputValidatorRegex.update_forward_refs()
 DivLinearGradient.update_forward_refs()
 DivMatchParentSize.update_forward_refs()
 DivNeighbourPageSize.update_forward_refs()
 DivNinePatchBackground.update_forward_refs()
 DivPageSize.update_forward_refs()
 DivPager.update_forward_refs()
 DivPatch.update_forward_refs()
@@ -167,37 +205,46 @@
 DivPoint.update_forward_refs()
 DivRadialGradient.update_forward_refs()
 DivRadialGradientFixedCenter.update_forward_refs()
 DivRadialGradientRelativeCenter.update_forward_refs()
 DivRadialGradientRelativeRadius.update_forward_refs()
 DivRoundedRectangleShape.update_forward_refs()
 DivScaleTransition.update_forward_refs()
+DivSelect.update_forward_refs()
+DivSelectOption.update_forward_refs()
 DivSeparator.update_forward_refs()
 DivSeparatorDelimiterStyle.update_forward_refs()
 DivShadow.update_forward_refs()
 DivShapeDrawable.update_forward_refs()
 DivSlideTransition.update_forward_refs()
 DivSlider.update_forward_refs()
 DivSliderTextStyle.update_forward_refs()
 DivSolidBackground.update_forward_refs()
 DivState.update_forward_refs()
 DivStateState.update_forward_refs()
+DivStretchIndicatorItemPlacement.update_forward_refs()
 DivStroke.update_forward_refs()
 DivTabs.update_forward_refs()
 DivTabsItem.update_forward_refs()
 DivTabsTabTitleStyle.update_forward_refs()
 DivText.update_forward_refs()
 DivTextEllipsis.update_forward_refs()
 DivTextImage.update_forward_refs()
 DivTextRange.update_forward_refs()
+DivTextRangeBorder.update_forward_refs()
+DivTimer.update_forward_refs()
 DivTooltip.update_forward_refs()
 DivTransform.update_forward_refs()
 DivTransitionBase.update_forward_refs()
 DivTrigger.update_forward_refs()
+DivVideo.update_forward_refs()
+DivVideoSource.update_forward_refs()
+DivVideoSourceResolution.update_forward_refs()
 DivVisibilityAction.update_forward_refs()
 DivWrapContentSize.update_forward_refs()
+DivWrapContentSizeConstraintSize.update_forward_refs()
 IntegerVariable.update_forward_refs()
 NumberVariable.update_forward_refs()
 StringVariable.update_forward_refs()
 UrlVariable.update_forward_refs()
 
-__all__ = ("BooleanVariable", "ColorVariable", "DelimiterStyleOrientation", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionMenuItem", "DivActionTarget", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivCornersRadius", "DivCount", "DivCustom", "DivData", "DivDataState", "DivDimension", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFixedCount", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontFamily", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputNativeInterface", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextTruncate", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivVariable", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "IntegerVariable", "NumberVariable", "StringVariable", "TabTitleStyleAnimationType", "UrlVariable")
+__all__ = ("BooleanVariable", "ColorVariable", "DelimiterStyleOrientation", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionMenuItem", "DivActionTarget", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBlur", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivCornersRadius", "DivCount", "DivCurrencyInputMask", "DivCustom", "DivData", "DivDataState", "DivDefaultIndicatorItemPlacement", "DivDimension", "DivDisappearAction", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFilter", "DivFixedCount", "DivFixedLengthInputMask", "DivFixedLengthInputMaskPatternElement", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontFamily", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivIndicatorItemPlacement", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputMask", "DivInputMaskBase", "DivInputNativeInterface", "DivInputValidator", "DivInputValidatorBase", "DivInputValidatorExpression", "DivInputValidatorRegex", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSelect", "DivSelectOption", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStretchIndicatorItemPlacement", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextRangeBackground", "DivTextRangeBorder", "DivTextTruncate", "DivTimer", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivVariable", "DivVideo", "DivVideoSource", "DivVideoSourceResolution", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "DivWrapContentSizeConstraintSize", "IntegerVariable", "NumberVariable", "StringVariable", "TabTitleStyleAnimationType", "UrlVariable")
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/boolean_variable.py` & `pydivkit-25.6.0/pydivkit/div/boolean_variable.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
 # A Boolean variable in binary format.
 class BooleanVariable(BaseDiv):
 
     def __init__(
         self, *,
-        name: str,
-        value: bool,
         type: str = "boolean",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Union[Expr, bool]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             name=name,
             value=value,
+            **kwargs,
         )
 
     type: str = Field(default="boolean")
-    name: str = Field(
+    name: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Variable name.",
     )
-    value: bool = Field(
+    value: typing.Union[Expr, bool] = Field(
         description="Value.",
     )
 
 
 BooleanVariable.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/color_variable.py` & `pydivkit-25.6.0/pydivkit/div/string_variable.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
-# Variable — HEX color as a string.
-class ColorVariable(BaseDiv):
+# A string variable.
+class StringVariable(BaseDiv):
 
     def __init__(
         self, *,
-        name: str,
-        value: str,
-        type: str = "color",
+        type: str = "string",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             name=name,
             value=value,
+            **kwargs,
         )
 
-    type: str = Field(default="color")
-    name: str = Field(
+    type: str = Field(default="string")
+    name: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Variable name.",
     )
-    value: str = Field(
-        format="color", 
+    value: typing.Union[Expr, str] = Field(
         description="Value.",
     )
 
 
-ColorVariable.update_forward_refs()
+StringVariable.update_forward_refs()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div.py` & `pydivkit-25.6.0/pydivkit/div/div.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from __future__ import annotations
 
 import enum
 import typing
 from typing import Union
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_container, div_custom, div_gallery, div_gif_image, div_grid, div_image,
-    div_indicator, div_input, div_pager, div_separator, div_slider, div_state,
-    div_tabs, div_text,
+    div_indicator, div_input, div_pager, div_select, div_separator, div_slider,
+    div_state, div_tabs, div_text, div_video,
 )
 
 
 Div = Union[
     div_image.DivImage,
     div_gif_image.DivGifImage,
     div_text.DivText,
@@ -27,8 +27,10 @@
     div_pager.DivPager,
     div_tabs.DivTabs,
     div_state.DivState,
     div_custom.DivCustom,
     div_indicator.DivIndicator,
     div_slider.DivSlider,
     div_input.DivInput,
+    div_select.DivSelect,
+    div_video.DivVideo,
 ]
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_absolute_edge_insets.py` & `pydivkit-25.6.0/pydivkit/div/div_extension.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,42 +2,35 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
-# Sets the margins, without taking the properties of the screen.
-class DivAbsoluteEdgeInsets(BaseDiv):
+# Extension that affects an element.
+class DivExtension(BaseDiv):
 
     def __init__(
         self, *,
-        bottom: typing.Optional[int] = None,
-        left: typing.Optional[int] = None,
-        right: typing.Optional[int] = None,
-        top: typing.Optional[int] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            bottom=bottom,
-            left=left,
-            right=right,
-            top=top,
+            id=id,
+            params=params,
+            **kwargs,
         )
 
-    bottom: typing.Optional[int] = Field(
-        description="Bottom margin.",
+    id: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description="Extension ID.",
     )
-    left: typing.Optional[int] = Field(
-        description="Left margin.",
-    )
-    right: typing.Optional[int] = Field(
-        description="Right margin.",
-    )
-    top: typing.Optional[int] = Field(
-        description="Top margin.",
+    params: typing.Optional[typing.Dict[str, typing.Any]] = Field(
+        description="Additional extension parameters.",
     )
 
 
-DivAbsoluteEdgeInsets.update_forward_refs()
+DivExtension.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_accessibility.py` & `pydivkit-25.6.0/pydivkit/div/div_accessibility.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,80 +2,83 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
-# Accessibility for disabled people.
+# Accessibility settings.
 class DivAccessibility(BaseDiv):
 
     def __init__(
         self, *,
-        description: typing.Optional[str] = None,
-        hint: typing.Optional[str] = None,
-        mode: typing.Optional[DivAccessibilityMode] = None,
-        mute_after_action: typing.Optional[bool] = None,
-        state_description: typing.Optional[str] = None,
-        type: typing.Optional[DivAccessibilityType] = None,
+        description: typing.Optional[typing.Union[Expr, str]] = None,
+        hint: typing.Optional[typing.Union[Expr, str]] = None,
+        mode: typing.Optional[typing.Union[Expr, DivAccessibilityMode]] = None,
+        mute_after_action: typing.Optional[typing.Union[Expr, bool]] = None,
+        state_description: typing.Optional[typing.Union[Expr, str]] = None,
+        type: typing.Optional[typing.Union[Expr, DivAccessibilityType]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             description=description,
             hint=hint,
             mode=mode,
             mute_after_action=mute_after_action,
             state_description=state_description,
             type=type,
+            **kwargs,
         )
 
-    description: typing.Optional[str] = Field(
+    description: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element description. It is used as the main description for "
             "screen readingapplications."
         ),
     )
-    hint: typing.Optional[str] = Field(
+    hint: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "A tooltip of what will happen during interaction. If Speak "
             "Hints is enabled inthe VoiceOver settings on iOS, a tooltip "
             "is played after `description`."
         ),
     )
-    mode: typing.Optional[DivAccessibilityMode] = Field(
+    mode: typing.Optional[typing.Union[Expr, DivAccessibilityMode]] = Field(
         description=(
             "The way the accessibility tree is organized. In the `merge` "
             "mode theaccessibility service perceives an element together "
             "with a subtree as a whole. Inthe `exclude` mode an element "
             "together with a subtree isn\'t available foraccessibility."
         ),
     )
-    mute_after_action: typing.Optional[bool] = Field(
+    mute_after_action: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
-            "Mutes the sound of the screen reader after interacting with "
-            "the element."
+            "Mutes the screen reader sound after interacting with the "
+            "element."
         ),
     )
-    state_description: typing.Optional[str] = Field(
+    state_description: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Description of the current state of an element. For "
             "example, in the descriptionyou can specify a selected date "
             "for a date selection element and an on/off statefor a "
             "switch."
         ),
     )
-    type: typing.Optional[DivAccessibilityType] = Field(
+    type: typing.Optional[typing.Union[Expr, DivAccessibilityType]] = Field(
         description=(
-            "Element role. It is used for correct identification of an "
-            "element by anaccessibility service."
+            "Element role. Used to correctly identify an element by the "
+            "accessibility service.For example, the `list` element is "
+            "used to group list elements into one element."
         ),
     )
 
 
 class DivAccessibilityMode(str, enum.Enum):
     DEFAULT = "default"
     MERGE = "merge"
@@ -86,10 +89,11 @@
     NONE = "none"
     BUTTON = "button"
     IMAGE = "image"
     TEXT = "text"
     EDIT_TEXT = "edit_text"
     HEADER = "header"
     TAB_BAR = "tab_bar"
+    LIST = "list"
 
 
 DivAccessibility.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_action.py` & `pydivkit-25.6.0/pydivkit/div/div_focus.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,114 +2,98 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_download_callbacks
+from . import div_action, div_background, div_border
 
 
-# It defines an action when clicking on an element.
-class DivAction(BaseDiv):
+# Element behavior when focusing or losing focus.
+class DivFocus(BaseDiv):
 
     def __init__(
         self, *,
-        log_id: str,
-        download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = None,
-        log_url: typing.Optional[str] = None,
-        menu_items: typing.Optional[typing.List[DivActionMenuItem]] = None,
-        payload: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        referer: typing.Optional[str] = None,
-        target: typing.Optional[DivActionTarget] = None,
-        url: typing.Optional[str] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
+        border: typing.Optional[div_border.DivBorder] = None,
+        next_focus_ids: typing.Optional[DivFocusNextFocusIds] = None,
+        on_blur: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        on_focus: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            download_callbacks=download_callbacks,
-            log_id=log_id,
-            log_url=log_url,
-            menu_items=menu_items,
-            payload=payload,
-            referer=referer,
-            target=target,
-            url=url,
+            background=background,
+            border=border,
+            next_focus_ids=next_focus_ids,
+            on_blur=on_blur,
+            on_focus=on_focus,
+            **kwargs,
         )
 
-    download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
+        min_items=1, 
         description=(
-            "Callbacks that are called after "
-            "[dataloading](../../interaction.dita#loading-data)."
+            "Background of an element when it is in focus. It can "
+            "contain multiple layers."
         ),
     )
-    log_id: str = Field(
-        min_length=1, 
-        description="Logging ID.",
-    )
-    log_url: typing.Optional[str] = Field(
-        format="uri", 
-        description="URL for logging.",
-    )
-    menu_items: typing.Optional[typing.List[DivActionMenuItem]] = Field(
-        min_items=1, 
-        description="Context menu.",
-    )
-    payload: typing.Optional[typing.Dict[str, typing.Any]] = Field(
-        description="Additional parameters, passed to the host application.",
+    border: typing.Optional[div_border.DivBorder] = Field(
+        description="Border of an element when it\'s in focus.",
     )
-    referer: typing.Optional[str] = Field(
-        format="uri", 
-        description="Referer URL for logging.",
+    next_focus_ids: typing.Optional[DivFocusNextFocusIds] = Field(
+        description="IDs of elements that will be next to get focus.",
     )
-    target: typing.Optional[DivActionTarget] = Field(
-        description="The tab in which the URL must be opened.",
+    on_blur: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Actions when an element loses focus.",
     )
-    url: typing.Optional[str] = Field(
-        format="uri", 
-        description=(
-            "URL. Possible values: `url` or `div-action://`. To learn "
-            "more, see [Interactionwith "
-            "elements](../../interaction.dita)."
-        ),
+    on_focus: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Actions when an element gets focus.",
     )
 
 
-class DivActionTarget(str, enum.Enum):
-    SELF = "_self"
-    BLANK = "_blank"
-
-
-class DivActionMenuItem(BaseDiv):
+# IDs of elements that will be next to get focus.
+class DivFocusNextFocusIds(BaseDiv):
 
     def __init__(
         self, *,
-        text: str,
-        action: typing.Optional[DivAction] = None,
-        actions: typing.Optional[typing.List[DivAction]] = None,
+        down: typing.Optional[typing.Union[Expr, str]] = None,
+        forward: typing.Optional[typing.Union[Expr, str]] = None,
+        left: typing.Optional[typing.Union[Expr, str]] = None,
+        right: typing.Optional[typing.Union[Expr, str]] = None,
+        up: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            action=action,
-            actions=actions,
-            text=text,
+            down=down,
+            forward=forward,
+            left=left,
+            right=right,
+            up=up,
+            **kwargs,
         )
 
-    action: typing.Optional[DivAction] = Field(
-        description=(
-            "One action when clicking on a menu item. Not used if the "
-            "`actions` parameter isset."
-        ),
+    down: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1,
     )
-    actions: typing.Optional[typing.List[DivAction]] = Field(
-        min_items=1, 
-        description="Multiple actions when clicking on a menu item.",
+    forward: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1,
+    )
+    left: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1,
+    )
+    right: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1,
     )
-    text: str = Field(
-        min_length=1, 
-        description="Menu item title.",
+    up: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1,
     )
 
 
-DivActionMenuItem.update_forward_refs()
+DivFocusNextFocusIds.update_forward_refs()
 
 
-DivAction.update_forward_refs()
+DivFocus.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_animation.py` & `pydivkit-25.6.0/pydivkit/div/div_tooltip.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,82 +2,94 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_animation_interpolator, div_count
+from . import div, div_animation, div_point
 
 
-# Element animation parameters.
-class DivAnimation(BaseDiv):
+# Tooltip.
+class DivTooltip(BaseDiv):
 
     def __init__(
         self, *,
-        name: DivAnimationName,
-        duration: typing.Optional[int] = None,
-        end_value: typing.Optional[float] = None,
-        interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = None,
-        items: typing.Optional[typing.List[DivAnimation]] = None,
-        repeat: typing.Optional[div_count.DivCount] = None,
-        start_delay: typing.Optional[int] = None,
-        start_value: typing.Optional[float] = None,
+        animation_in: typing.Optional[div_animation.DivAnimation] = None,
+        animation_out: typing.Optional[div_animation.DivAnimation] = None,
+        div: typing.Optional[div.Div] = None,
+        duration: typing.Optional[typing.Union[Expr, int]] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        offset: typing.Optional[div_point.DivPoint] = None,
+        position: typing.Optional[typing.Union[Expr, DivTooltipPosition]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
+            animation_in=animation_in,
+            animation_out=animation_out,
+            div=div,
             duration=duration,
-            end_value=end_value,
-            interpolator=interpolator,
-            items=items,
-            name=name,
-            repeat=repeat,
-            start_delay=start_delay,
-            start_value=start_value,
+            id=id,
+            offset=offset,
+            position=position,
+            **kwargs,
         )
 
-    duration: typing.Optional[int] = Field(
-        description="Animation duration in milliseconds.",
-    )
-    end_value: typing.Optional[float] = Field(
-        description="Final value of an animation.",
+    animation_in: typing.Optional[div_animation.DivAnimation] = Field(
+        description=(
+            "Tooltip appearance animation. By default, the tooltip will "
+            "be appearing graduallywith an offset from the anchor point "
+            "by 10 dp."
+        ),
     )
-    interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = Field(
+    animation_out: typing.Optional[div_animation.DivAnimation] = Field(
         description=(
-            "Animation speed nature. When the value is set to `spring` — "
-            "animation of dampingfluctuations cut to 0.7 with the "
-            "`damping=1` parameter. Other options correspondto the "
-            "Bezier curve:`linear` — cubic-bezier(0, 0, 1, 1);`ease` "
-            "—cubic-bezier(0.25, 0.1, 0.25, 1);`ease_in` — "
-            "cubic-bezier(0.42, 0, 1,1);`ease_out` — cubic-bezier(0, 0, "
-            "0.58, 1);`ease_in_out` — cubic-bezier(0.42, 0,0.58, 1)."
+            "Tooltip disappearance animation. By default, the tooltip "
+            "will disappear graduallywith an offset from the anchor "
+            "point by 10 dp."
         ),
     )
-    items: typing.Optional[typing.List[DivAnimation]] = Field(
-        min_items=1, 
-        description="Animation elements.",
+    div: div.Div = Field(
+        description=(
+            "An element that will be shown in a tooltip. If there are "
+            "tooltips inside anelement, they won\'t be shown."
+        ),
     )
-    name: DivAnimationName = Field(
-        description="Animation type.",
+    duration: typing.Optional[typing.Union[Expr, int]] = Field(
+        description=(
+            "Duration of the tooltip visibility in milliseconds. When "
+            "the value is set to `0`,the tooltip will be visible until "
+            "the user hides it."
+        ),
     )
-    repeat: typing.Optional[div_count.DivCount] = Field(
-        description="Number of animation repetitions.",
+    id: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description=(
+            "Tooltip ID. It is used to avoid re-showing. It must be "
+            "unique for all elementtooltips."
+        ),
     )
-    start_delay: typing.Optional[int] = Field(
-        description="Delay in milliseconds before animation starts.",
+    offset: typing.Optional[div_point.DivPoint] = Field(
+        description="Shift relative to an anchor point.",
     )
-    start_value: typing.Optional[float] = Field(
-        description="Starting value of an animation.",
+    position: typing.Union[Expr, DivTooltipPosition] = Field(
+        description=(
+            "The position of a tooltip relative to an element it belongs "
+            "to."
+        ),
     )
 
 
-class DivAnimationName(str, enum.Enum):
-    FADE = "fade"
-    TRANSLATE = "translate"
-    SCALE = "scale"
-    NATIVE = "native"
-    SET = "set"
-    NO_ANIMATION = "no_animation"
+class DivTooltipPosition(str, enum.Enum):
+    LEFT = "left"
+    TOP_LEFT = "top-left"
+    TOP = "top"
+    TOP_RIGHT = "top-right"
+    RIGHT = "right"
+    BOTTOM_RIGHT = "bottom-right"
+    BOTTOM = "bottom"
+    BOTTOM_LEFT = "bottom-left"
 
 
-DivAnimation.update_forward_refs()
+DivTooltip.update_forward_refs()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_appearance_set_transition.py` & `pydivkit-25.6.0/pydivkit/div/div_appearance_set_transition.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_appearance_transition
 
 
 # A set of animations to be applied simultaneously.
 class DivAppearanceSetTransition(BaseDiv):
 
     def __init__(
         self, *,
-        items: typing.List[div_appearance_transition.DivAppearanceTransition],
         type: str = "set",
+        items: typing.Optional[typing.Sequence[div_appearance_transition.DivAppearanceTransition]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             items=items,
+            **kwargs,
         )
 
     type: str = Field(default="set")
-    items: typing.List[div_appearance_transition.DivAppearanceTransition] = Field(
+    items: typing.Sequence[div_appearance_transition.DivAppearanceTransition] = Field(
         min_items=1, 
         description="An array of animations.",
     )
 
 
 DivAppearanceSetTransition.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_appearance_transition.py` & `pydivkit-25.6.0/pydivkit/div/div_appearance_transition.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import enum
 import typing
 from typing import Union
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_appearance_set_transition, div_fade_transition, div_scale_transition,
     div_slide_transition,
 )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_background.py` & `pydivkit-25.6.0/pydivkit/div/div_background.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import enum
 import typing
 from typing import Union
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_image_background, div_linear_gradient, div_nine_patch_background,
     div_radial_gradient, div_solid_background,
 )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_base.py` & `pydivkit-25.6.0/pydivkit/div/div_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,63 +2,66 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_edge_insets, div_extension,
-    div_focus, div_size, div_tooltip, div_transform, div_transition_trigger,
-    div_visibility, div_visibility_action,
+    div_border, div_change_transition, div_disappear_action, div_edge_insets,
+    div_extension, div_focus, div_size, div_tooltip, div_transform,
+    div_transition_trigger, div_visibility, div_visibility_action,
 )
 
 
 class DivBase(BaseDiv):
 
     def __init__(
         self, *,
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        row_span: typing.Optional[int] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             accessibility=accessibility,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
             background=background,
             border=border,
             column_span=column_span,
+            disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
             margins=margins,
             paddings=paddings,
             row_span=row_span,
@@ -69,50 +72,55 @@
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
@@ -124,53 +132,52 @@
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -186,31 +193,31 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_border.py` & `pydivkit-25.6.0/pydivkit/div/div_rounded_rectangle_shape.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,52 +2,55 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_corners_radius, div_shadow, div_stroke
+from . import div_fixed_size, div_stroke
 
 
-# Stroke around the element.
-class DivBorder(BaseDiv):
+# A rectangle with rounded corners.
+class DivRoundedRectangleShape(BaseDiv):
 
     def __init__(
         self, *,
-        corner_radius: typing.Optional[int] = None,
-        corners_radius: typing.Optional[div_corners_radius.DivCornersRadius] = None,
-        has_shadow: typing.Optional[bool] = None,
-        shadow: typing.Optional[div_shadow.DivShadow] = None,
+        type: str = "rounded_rectangle",
+        background_color: typing.Optional[typing.Union[Expr, str]] = None,
+        corner_radius: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        item_height: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        item_width: typing.Optional[div_fixed_size.DivFixedSize] = None,
         stroke: typing.Optional[div_stroke.DivStroke] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
+            type=type,
+            background_color=background_color,
             corner_radius=corner_radius,
-            corners_radius=corners_radius,
-            has_shadow=has_shadow,
-            shadow=shadow,
+            item_height=item_height,
+            item_width=item_width,
             stroke=stroke,
+            **kwargs,
         )
 
-    corner_radius: typing.Optional[int] = Field(
-        description=(
-            "One radius of element and stroke corner rounding. Has a "
-            "lower priority than`corners_radius`."
-        ),
+    type: str = Field(default="rounded_rectangle")
+    background_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Fill color.",
     )
-    corners_radius: typing.Optional[div_corners_radius.DivCornersRadius] = Field(
-        description="Multiple radii of element and stroke corner rounding.",
+    corner_radius: typing.Optional[div_fixed_size.DivFixedSize] = Field(
+        description="Corner rounding radius.",
     )
-    has_shadow: typing.Optional[bool] = Field(
-        description="Adding shadow.",
+    item_height: typing.Optional[div_fixed_size.DivFixedSize] = Field(
+        description="Height.",
     )
-    shadow: typing.Optional[div_shadow.DivShadow] = Field(
-        description="Shadow parameters.",
+    item_width: typing.Optional[div_fixed_size.DivFixedSize] = Field(
+        description="Width.",
     )
     stroke: typing.Optional[div_stroke.DivStroke] = Field(
         description="Stroke style.",
     )
 
 
-DivBorder.update_forward_refs()
+DivRoundedRectangleShape.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_change_bounds_transition.py` & `pydivkit-25.6.0/pydivkit/div/div_change_bounds_transition.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_animation_interpolator
 
 
 # Element position and size change animation.
 class DivChangeBoundsTransition(BaseDiv):
 
     def __init__(
         self, *,
         type: str = "change_bounds",
-        duration: typing.Optional[int] = None,
-        interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = None,
-        start_delay: typing.Optional[int] = None,
+        duration: typing.Optional[typing.Union[Expr, int]] = None,
+        interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = None,
+        start_delay: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             duration=duration,
             interpolator=interpolator,
             start_delay=start_delay,
+            **kwargs,
         )
 
     type: str = Field(default="change_bounds")
-    duration: typing.Optional[int] = Field(
+    duration: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Animation duration in milliseconds.",
     )
-    interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = Field(
+    interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = Field(
         description="Transition speed nature.",
     )
-    start_delay: typing.Optional[int] = Field(
+    start_delay: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Delay in milliseconds before animation starts.",
     )
 
 
 DivChangeBoundsTransition.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_circle_shape.py` & `pydivkit-25.6.0/pydivkit/div/div_fixed_count.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_fixed_size
 
-
-# A circle.
-class DivCircleShape(BaseDiv):
+# Fixed number of repetitions.
+class DivFixedCount(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "circle",
-        radius: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        type: str = "fixed",
+        value: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            radius=radius,
+            value=value,
+            **kwargs,
         )
 
-    type: str = Field(default="circle")
-    radius: typing.Optional[div_fixed_size.DivFixedSize] = Field(
-        description="Radius.",
+    type: str = Field(default="fixed")
+    value: typing.Union[Expr, int] = Field(
+        description="Number of repetitions.",
     )
 
 
-DivCircleShape.update_forward_refs()
+DivFixedCount.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_container.py` & `pydivkit-25.6.0/pydivkit/div/div_grid.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,184 +2,177 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_animation, div_appearance_transition,
-    div_background, div_border, div_change_transition, div_drawable,
+    div_background, div_border, div_change_transition, div_disappear_action,
     div_edge_insets, div_extension, div_focus, div_size, div_tooltip,
     div_transform, div_transition_trigger, div_visibility,
     div_visibility_action,
 )
 
 
-# Container. It contains other elements and is responsible for their location. It
-# is used to arrange elements vertically, horizontally, and with an overlay in a
-# certain order, simulating the third dimension.
-class DivContainer(BaseDiv):
+# A grid with an option to merge cells vertically and horizontally.
+class DivGrid(BaseDiv):
 
     def __init__(
         self, *,
-        items: typing.List[div.Div],
-        type: str = "container",
+        type: str = "grid",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
         action: typing.Optional[div_action.DivAction] = None,
         action_animation: typing.Optional[div_animation.DivAnimation] = None,
-        actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        doubletap_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_count: typing.Optional[typing.Union[Expr, int]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
-        layout_mode: typing.Optional[DivContainerLayoutMode] = None,
-        line_separator: typing.Optional[DivContainerSeparator] = None,
-        longtap_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        items: typing.Optional[typing.Sequence[div.Div]] = None,
+        longtap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        orientation: typing.Optional[DivContainerOrientation] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        row_span: typing.Optional[int] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        separator: typing.Optional[DivContainerSeparator] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
             action=action,
             action_animation=action_animation,
             actions=actions,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
             background=background,
             border=border,
+            column_count=column_count,
             column_span=column_span,
             content_alignment_horizontal=content_alignment_horizontal,
             content_alignment_vertical=content_alignment_vertical,
+            disappear_actions=disappear_actions,
             doubletap_actions=doubletap_actions,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
             items=items,
-            layout_mode=layout_mode,
-            line_separator=line_separator,
             longtap_actions=longtap_actions,
             margins=margins,
-            orientation=orientation,
             paddings=paddings,
             row_span=row_span,
             selected_actions=selected_actions,
-            separator=separator,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="container")
+    type: str = Field(default="grid")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
     action: typing.Optional[div_action.DivAction] = Field(
         description=(
             "One action when clicking on an element. Not used if the "
             "`actions` parameter isset."
         ),
     )
     action_animation: typing.Optional[div_animation.DivAnimation] = Field(
         description=(
-            "Action animation. Web supports `fade`, `scale` and `set` "
-            "only."
+            "Click animation. The web only supports the following "
+            "values: `fade`, `scale`,`native`, `no_animation` and `set`."
         ),
     )
-    actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description="Multiple actions when clicking on an element.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_count: typing.Union[Expr, int] = Field(
+        description="Number of columns.",
+    )
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
-        description=(
-            "Default alignment of elements. Not used if the "
-            "`alignment_horizontal` parameteris set from the element "
-            "field."
-        ),
+    content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
+        description="Horizontal alignment of grid contents.",
     )
-    content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
-        description=(
-            "Default alignment of elements. `baseline` value aligns "
-            "elements having their ownbaseline along this baseline. "
-            "Other elements are aligned by top side in thiscase. Not "
-            "used if the `alignment_vertical` parameter is set from the "
-            "elementfield."
-        ),
+    content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
+        description="Vertical alignment of grid contents.",
     )
-    doubletap_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description="Action when double-clicking on an element.",
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
@@ -191,94 +184,63 @@
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    items: typing.List[div.Div] = Field(
+    items: typing.Sequence[div.Div] = Field(
         min_items=1, 
-        description="Nested elements.",
-    )
-    layout_mode: typing.Optional[DivContainerLayoutMode] = Field(
-        description=(
-            "Method of placing elements. `wrap` value includes the "
-            "transfer of elements to thenext line if they did not fit in "
-            "the previous one. If the value is set to `wrap`,then a "
-            "separate line will be allocated for all elements with a "
-            "size value of`match_parent` along the main axis. If the "
-            "value is set to `wrap`, then elementswith a size value of "
-            "`match_parent` along the cross axis will be ignored."
-        ),
+        description="Contents.",
     )
-    line_separator: typing.Optional[DivContainerSeparator] = Field(
-        description=(
-            "Separator between elements along the cross axis. Not used "
-            "if the `layout_mode`parameter has the value `no_wrap\'."
-        ),
-    )
-    longtap_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    longtap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
-            "Action when long-clicking on an element. Doesn\'t work on "
-            "the devices w/o touchgestures."
+            "Action when long-clicking an element. Doesn\'t work on "
+            "devices that don\'t supporttouch gestures."
         ),
     )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
-    orientation: typing.Optional[DivContainerOrientation] = Field(
-        description=(
-            "Location of elements. `overlap` value overlays elements on "
-            "top of each other inthe order of enumeration. The lowest is "
-            "the zero element of an array."
-        ),
-    )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    separator: typing.Optional[DivContainerSeparator] = Field(
-        description=(
-            "Separator between elements along the main axis. Not used if "
-            "the `orientation`parameter has the value `overlap\'."
-        ),
-    )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -294,77 +256,33 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-class DivContainerLayoutMode(str, enum.Enum):
-    NO_WRAP = "no_wrap"
-    WRAP = "wrap"
-
-
-class DivContainerOrientation(str, enum.Enum):
-    VERTICAL = "vertical"
-    HORIZONTAL = "horizontal"
-    OVERLAP = "overlap"
-
-
-class DivContainerSeparator(BaseDiv):
-
-    def __init__(
-        self, *,
-        style: div_drawable.DivDrawable,
-        show_at_end: typing.Optional[bool] = None,
-        show_at_start: typing.Optional[bool] = None,
-        show_between: typing.Optional[bool] = None,
-    ):
-        super().__init__(
-            show_at_end=show_at_end,
-            show_at_start=show_at_start,
-            show_between=show_between,
-            style=style,
-        )
-
-    show_at_end: typing.Optional[bool] = Field(
-        description="Enables showing of separator after the last item.",
-    )
-    show_at_start: typing.Optional[bool] = Field(
-        description="Enables showing of separator before the first item.",
-    )
-    show_between: typing.Optional[bool] = Field(
-        description="Enables showing of separator between items.",
-    )
-    style: div_drawable.DivDrawable = Field(
-        description="Style of the separator.",
-    )
-
-
-DivContainerSeparator.update_forward_refs()
-
-
-DivContainer.update_forward_refs()
+DivGrid.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_corners_radius.py` & `pydivkit-25.6.0/pydivkit/div/div_corners_radius.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,59 +2,61 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
 # Sets corner rounding.
 class DivCornersRadius(BaseDiv):
 
     def __init__(
         self, *,
-        bottom_left: typing.Optional[int] = None,
-        bottom_right: typing.Optional[int] = None,
-        top_left: typing.Optional[int] = None,
-        top_right: typing.Optional[int] = None,
+        bottom_left: typing.Optional[typing.Union[Expr, int]] = None,
+        bottom_right: typing.Optional[typing.Union[Expr, int]] = None,
+        top_left: typing.Optional[typing.Union[Expr, int]] = None,
+        top_right: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             bottom_left=bottom_left,
             bottom_right=bottom_right,
             top_left=top_left,
             top_right=top_right,
+            **kwargs,
         )
 
-    bottom_left: typing.Optional[int] = Field(
+    bottom_left: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Rounding radius of a lower left corner. If not specified, "
             "then `corner_radius` isused."
         )
         , 
         name="bottom-left",
     )
-    bottom_right: typing.Optional[int] = Field(
+    bottom_right: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Rounding radius of a lower right corner. If not specified, "
             "then `corner_radius`is used."
         )
         , 
         name="bottom-right",
     )
-    top_left: typing.Optional[int] = Field(
+    top_left: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Rounding radius of an upper left corner. If not specified, "
             "then `corner_radius`is used."
         )
         , 
         name="top-left",
     )
-    top_right: typing.Optional[int] = Field(
+    top_right: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Rounding radius of an upper right corner. If not specified, "
             "then `corner_radius`is used."
         )
         , 
         name="top-right",
     )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_custom.py` & `pydivkit-25.6.0/pydivkit/div/div_custom.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,72 +2,75 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_edge_insets, div_extension,
-    div_focus, div_size, div_tooltip, div_transform, div_transition_trigger,
-    div_visibility, div_visibility_action,
+    div_border, div_change_transition, div_disappear_action, div_edge_insets,
+    div_extension, div_focus, div_size, div_tooltip, div_transform,
+    div_transition_trigger, div_visibility, div_visibility_action,
 )
 
 
 # Custom element. It is delegated to a host application to create native elements
 # depending on the platform.
 class DivCustom(BaseDiv):
 
     def __init__(
         self, *,
-        custom_type: str,
         type: str = "custom",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
         custom_props: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        custom_type: typing.Optional[typing.Union[Expr, str]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
-        items: typing.Optional[typing.List[div.Div]] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        items: typing.Optional[typing.Sequence[div.Div]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        row_span: typing.Optional[int] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
             background=background,
             border=border,
             column_span=column_span,
             custom_props=custom_props,
             custom_type=custom_type,
+            disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
             items=items,
             margins=margins,
             paddings=paddings,
@@ -79,57 +82,62 @@
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
     type: str = Field(default="custom")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
     custom_props: typing.Optional[typing.Dict[str, typing.Any]] = Field(
         description="Element data for a host application.",
     )
-    custom_type: str = Field(
+    custom_type: typing.Union[Expr, str] = Field(
         description="Subtype of an element for a host application.",
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
@@ -141,57 +149,56 @@
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    items: typing.Optional[typing.List[div.Div]] = Field(
+    items: typing.Optional[typing.Sequence[div.Div]] = Field(
         min_items=1, 
         description="Nested elements.",
     )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -207,31 +214,31 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_data.py` & `pydivkit-25.6.0/pydivkit/div/div_input_validator_regex.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,81 +2,53 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div, div_transition_selector, div_trigger, div_variable
 
-
-# Root structure.
-class DivData(BaseDiv):
+# Regex validator.
+class DivInputValidatorRegex(BaseDiv):
 
     def __init__(
         self, *,
-        log_id: str,
-        states: typing.List[DivDataState],
-        transition_animation_selector: typing.Optional[div_transition_selector.DivTransitionSelector] = None,
-        variable_triggers: typing.Optional[typing.List[div_trigger.DivTrigger]] = None,
-        variables: typing.Optional[typing.List[div_variable.DivVariable]] = None,
+        type: str = "regex",
+        allow_empty: typing.Optional[typing.Union[Expr, bool]] = None,
+        label_id: typing.Optional[typing.Union[Expr, str]] = None,
+        pattern: typing.Optional[typing.Union[Expr, str]] = None,
+        variable: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            log_id=log_id,
-            states=states,
-            transition_animation_selector=transition_animation_selector,
-            variable_triggers=variable_triggers,
-            variables=variables,
+            type=type,
+            allow_empty=allow_empty,
+            label_id=label_id,
+            pattern=pattern,
+            variable=variable,
+            **kwargs,
         )
 
-    log_id: str = Field(
-        min_length=1, 
-        description="Logging ID.",
+    type: str = Field(default="regex")
+    allow_empty: typing.Optional[typing.Union[Expr, bool]] = Field(
+        description="Whether an empty value is correct. By default, false.",
     )
-    states: typing.List[DivDataState] = Field(
-        min_items=1, 
+    label_id: typing.Union[Expr, str] = Field(
+        min_length=1, 
         description=(
-            "A set of visual element states. Each element can have a few "
-            "states with adifferent layout. The states are displayed "
-            "strictly one by one and switched "
-            "using[action](div-action.md)."
+            "ID of the text div containing the error message, which will "
+            "also be used foraccessibility."
         ),
     )
-    transition_animation_selector: typing.Optional[div_transition_selector.DivTransitionSelector] = Field(
-        description="Events that trigger transition animations. @deprecated",
-    )
-    variable_triggers: typing.Optional[typing.List[div_trigger.DivTrigger]] = Field(
-        min_items=1, 
-        description="Triggers for changing variables.",
-    )
-    variables: typing.Optional[typing.List[div_variable.DivVariable]] = Field(
-        min_items=1, 
-        description="Declaration of variables that can be used in an element.",
-    )
-
-
-class DivDataState(BaseDiv):
-
-    def __init__(
-        self, *,
-        div: div.Div,
-        state_id: int,
-    ):
-        super().__init__(
-            div=div,
-            state_id=state_id,
-        )
-
-    div: div.Div = Field(
-        description="Contents.",
+    pattern: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description="Regex pattern for matching.",
     )
-    state_id: int = Field(
-        description="State ID.",
+    variable: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description="Name of validation storage variable.",
     )
 
 
-DivDataState.update_forward_refs()
-
-
-DivData.update_forward_refs()
+DivInputValidatorRegex.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_fade_transition.py` & `pydivkit-25.6.0/pydivkit/div/div_transform.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,50 +2,44 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_animation_interpolator
+from . import div_pivot
 
 
-# Transparency animation.
-class DivFadeTransition(BaseDiv):
+# Transformation of the element.
+class DivTransform(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "fade",
-        alpha: typing.Optional[float] = None,
-        duration: typing.Optional[int] = None,
-        interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = None,
-        start_delay: typing.Optional[int] = None,
+        pivot_x: typing.Optional[div_pivot.DivPivot] = None,
+        pivot_y: typing.Optional[div_pivot.DivPivot] = None,
+        rotation: typing.Optional[typing.Union[Expr, float]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            type=type,
-            alpha=alpha,
-            duration=duration,
-            interpolator=interpolator,
-            start_delay=start_delay,
+            pivot_x=pivot_x,
+            pivot_y=pivot_y,
+            rotation=rotation,
+            **kwargs,
         )
 
-    type: str = Field(default="fade")
-    alpha: typing.Optional[float] = Field(
-        description=(
-            "Value of the alpha channel which the element starts "
-            "appearing from or at which itfinishes disappearing."
-        ),
-    )
-    duration: typing.Optional[int] = Field(
-        description="Animation duration in milliseconds.",
+    pivot_x: typing.Optional[div_pivot.DivPivot] = Field(
+        description="X coordinate of the rotation axis.",
     )
-    interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = Field(
-        description="Transition speed nature.",
+    pivot_y: typing.Optional[div_pivot.DivPivot] = Field(
+        description="Y coordinate of the rotation axis.",
     )
-    start_delay: typing.Optional[int] = Field(
-        description="Delay in milliseconds before animation starts.",
+    rotation: typing.Optional[typing.Union[Expr, float]] = Field(
+        description=(
+            "Degrees of the element rotation. Positive values used for "
+            "clockwise rotation."
+        ),
     )
 
 
-DivFadeTransition.update_forward_refs()
+DivTransform.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_fixed_count.py` & `pydivkit-25.6.0/pydivkit/div/div_percentage_size.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
-# Fixed number of repetitions.
-class DivFixedCount(BaseDiv):
+# Element size (%).
+class DivPercentageSize(BaseDiv):
 
     def __init__(
         self, *,
-        value: int,
-        type: str = "fixed",
+        type: str = "percentage",
+        value: typing.Optional[typing.Union[Expr, float]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             value=value,
+            **kwargs,
         )
 
-    type: str = Field(default="fixed")
-    value: int = Field(
-        description="Number of repetitions.",
+    type: str = Field(default="percentage")
+    value: typing.Union[Expr, float] = Field(
+        description="Element size value.",
     )
 
 
-DivFixedCount.update_forward_refs()
+DivPercentageSize.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_fixed_size.py` & `pydivkit-25.6.0/pydivkit/div/div_pivot_fixed.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_size_unit
 
 
-# Fixed size of an element.
-class DivFixedSize(BaseDiv):
+# Fixed coordinates of the rotation axis.
+class DivPivotFixed(BaseDiv):
 
     def __init__(
         self, *,
-        value: int,
-        type: str = "fixed",
-        unit: typing.Optional[div_size_unit.DivSizeUnit] = None,
+        type: str = "pivot-fixed",
+        unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        value: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             unit=unit,
             value=value,
+            **kwargs,
         )
 
-    type: str = Field(default="fixed")
-    unit: typing.Optional[div_size_unit.DivSizeUnit] = Field(
+    type: str = Field(default="pivot-fixed")
+    unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description=(
-            "Unit of measurement. To learn more about units of size "
+            "Measurement unit. To learn more about units of size "
             "measurement, see [Layoutinside the "
             "card](../../layout.dita)."
         ),
     )
-    value: int = Field(
-        description="Element size.",
+    value: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Coordinate value.",
     )
 
 
-DivFixedSize.update_forward_refs()
+DivPivotFixed.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_focus.py` & `pydivkit-25.6.0/pydivkit/div/div_scale_transition.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,94 +2,68 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_action, div_background, div_border
+from . import div_animation_interpolator
 
 
-# Element behavior when focusing or losing focus.
-class DivFocus(BaseDiv):
+# Scale animation.
+class DivScaleTransition(BaseDiv):
 
     def __init__(
         self, *,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
-        border: typing.Optional[div_border.DivBorder] = None,
-        next_focus_ids: typing.Optional[DivFocusNextFocusIds] = None,
-        on_blur: typing.Optional[typing.List[div_action.DivAction]] = None,
-        on_focus: typing.Optional[typing.List[div_action.DivAction]] = None,
+        type: str = "scale",
+        duration: typing.Optional[typing.Union[Expr, int]] = None,
+        interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = None,
+        pivot_x: typing.Optional[typing.Union[Expr, float]] = None,
+        pivot_y: typing.Optional[typing.Union[Expr, float]] = None,
+        scale: typing.Optional[typing.Union[Expr, float]] = None,
+        start_delay: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            background=background,
-            border=border,
-            next_focus_ids=next_focus_ids,
-            on_blur=on_blur,
-            on_focus=on_focus,
+            type=type,
+            duration=duration,
+            interpolator=interpolator,
+            pivot_x=pivot_x,
+            pivot_y=pivot_y,
+            scale=scale,
+            start_delay=start_delay,
+            **kwargs,
         )
 
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
-        min_items=1, 
-        description=(
-            "Background of an element when it is in focus. It can "
-            "contain multiple layers."
-        ),
-    )
-    border: typing.Optional[div_border.DivBorder] = Field(
-        description="Border of an element when it is in focus",
+    type: str = Field(default="scale")
+    duration: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Animation duration in milliseconds.",
     )
-    next_focus_ids: typing.Optional[DivFocusNextFocusIds] = Field(
-        description="IDs of elements that will be next to get focus.",
+    interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = Field(
+        description="Transition speed nature.",
     )
-    on_blur: typing.Optional[typing.List[div_action.DivAction]] = Field(
-        min_items=1, 
-        description="Actions when an element loses focus.",
-    )
-    on_focus: typing.Optional[typing.List[div_action.DivAction]] = Field(
-        min_items=1, 
-        description="Actions when an element gets focus.",
-    )
-
-
-# IDs of elements that will be next to get focus.
-class DivFocusNextFocusIds(BaseDiv):
-
-    def __init__(
-        self, *,
-        down: typing.Optional[str] = None,
-        forward: typing.Optional[str] = None,
-        left: typing.Optional[str] = None,
-        right: typing.Optional[str] = None,
-        up: typing.Optional[str] = None,
-    ):
-        super().__init__(
-            down=down,
-            forward=forward,
-            left=left,
-            right=right,
-            up=up,
-        )
-
-    down: typing.Optional[str] = Field(
-        min_length=1,
-    )
-    forward: typing.Optional[str] = Field(
-        min_length=1,
+    pivot_x: typing.Optional[typing.Union[Expr, float]] = Field(
+        description=(
+            "Relative coordinate `X` of the point that won\'t change its "
+            "position in case ofscaling."
+        ),
     )
-    left: typing.Optional[str] = Field(
-        min_length=1,
+    pivot_y: typing.Optional[typing.Union[Expr, float]] = Field(
+        description=(
+            "Relative coordinate `Y` of the point that won\'t change its "
+            "position in case ofscaling."
+        ),
     )
-    right: typing.Optional[str] = Field(
-        min_length=1,
+    scale: typing.Optional[typing.Union[Expr, float]] = Field(
+        description=(
+            "Value of the scale from which the element starts appearing "
+            "or at which itfinishes disappearing."
+        ),
     )
-    up: typing.Optional[str] = Field(
-        min_length=1,
+    start_delay: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Delay in milliseconds before animation starts.",
     )
 
 
-DivFocusNextFocusIds.update_forward_refs()
-
-
-DivFocus.update_forward_refs()
+DivScaleTransition.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_gallery.py` & `pydivkit-25.6.0/pydivkit/div/div_separator.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,167 +2,165 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
-    div, div_accessibility, div_action, div_alignment_horizontal,
-    div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_edge_insets, div_extension,
-    div_focus, div_size, div_tooltip, div_transform, div_transition_trigger,
-    div_visibility, div_visibility_action,
+    div_accessibility, div_action, div_alignment_horizontal,
+    div_alignment_vertical, div_animation, div_appearance_transition,
+    div_background, div_border, div_change_transition, div_disappear_action,
+    div_edge_insets, div_extension, div_focus, div_size, div_tooltip,
+    div_transform, div_transition_trigger, div_visibility,
+    div_visibility_action,
 )
 
 
-# Gallery. It contains a horizontal or vertical set of cards that can be scrolled.
-class DivGallery(BaseDiv):
+# A separating line between elements.
+class DivSeparator(BaseDiv):
 
     def __init__(
         self, *,
-        items: typing.List[div.Div],
-        type: str = "gallery",
+        type: str = "separator",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        action: typing.Optional[div_action.DivAction] = None,
+        action_animation: typing.Optional[div_animation.DivAnimation] = None,
+        actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_count: typing.Optional[int] = None,
-        column_span: typing.Optional[int] = None,
-        cross_content_alignment: typing.Optional[DivGalleryCrossContentAlignment] = None,
-        cross_spacing: typing.Optional[int] = None,
-        default_item: typing.Optional[int] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        delimiter_style: typing.Optional[DivSeparatorDelimiterStyle] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
-        item_spacing: typing.Optional[int] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        longtap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        orientation: typing.Optional[DivGalleryOrientation] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        restrict_parent_scroll: typing.Optional[bool] = None,
-        row_span: typing.Optional[int] = None,
-        scroll_mode: typing.Optional[DivGalleryScrollMode] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
+            action=action,
+            action_animation=action_animation,
+            actions=actions,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
             background=background,
             border=border,
-            column_count=column_count,
             column_span=column_span,
-            cross_content_alignment=cross_content_alignment,
-            cross_spacing=cross_spacing,
-            default_item=default_item,
+            delimiter_style=delimiter_style,
+            disappear_actions=disappear_actions,
+            doubletap_actions=doubletap_actions,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
-            item_spacing=item_spacing,
-            items=items,
+            longtap_actions=longtap_actions,
             margins=margins,
-            orientation=orientation,
             paddings=paddings,
-            restrict_parent_scroll=restrict_parent_scroll,
             row_span=row_span,
-            scroll_mode=scroll_mode,
             selected_actions=selected_actions,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="gallery")
+    type: str = Field(default="separator")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
+    )
+    action: typing.Optional[div_action.DivAction] = Field(
+        description=(
+            "One action when clicking on an element. Not used if the "
+            "`actions` parameter isset."
+        ),
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    action_animation: typing.Optional[div_animation.DivAnimation] = Field(
+        description=(
+            "Click animation. The web only supports the following "
+            "values: `fade`, `scale`,`native`, `no_animation` and `set`."
+        ),
+    )
+    actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Multiple actions when clicking on an element.",
+    )
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_count: typing.Optional[int] = Field(
-        description="Number of columns for block layout.",
-    )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    cross_content_alignment: typing.Optional[DivGalleryCrossContentAlignment] = Field(
-        description=(
-            "Aligning elements in the direction perpendicular to the "
-            "scroll direction. Inhorizontal galleries:`start` — "
-            "alignment to the top of the card;`center` — to "
-            "thecenter;`end` — to the bottom.</p><p>In vertical "
-            "galleries:`start` — alignment tothe left of the "
-            "card;`center` — to the center;`end` — to the right."
-        ),
+    delimiter_style: typing.Optional[DivSeparatorDelimiterStyle] = Field(
+        description="Separator display settings.",
     )
-    cross_spacing: typing.Optional[int] = Field(
-        description=(
-            "Spacing between elements across the scroll axis. Default "
-            "value is `item_spacing`"
-        ),
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
     )
-    default_item: typing.Optional[int] = Field(
-        description=(
-            "Ordinal number of the gallery element to be scrolled to by "
-            "default. For`scroll_mode`:`default` — the scroll position "
-            "is set to the beginning of theelement, without taking into "
-            "account `item_spacing`;`paging` — the scrollposition is set "
-            "to the center of the element."
-        ),
+    doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Action when double-clicking on an element.",
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
@@ -174,91 +172,59 @@
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    item_spacing: typing.Optional[int] = Field(
-        description="Spacing between elements.",
-    )
-    items: typing.List[div.Div] = Field(
+    longtap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
-            "Gallery elements. Scrolling to elements can be "
-            "implementedusing:`div-action://set_current_item?id=&item=` "
-            "— scrolling to the element withan ordinal number `item` "
-            "inside an element, with the "
-            "specified`id`;`div-action://set_next_item?id=[&overflow={cl"
-            "amp|ring}]` — scrolling to thenext element inside an "
-            "element, with the "
-            "specified`id`;`div-action://set_previous_item?id=[&overflow"
-            "={clamp|ring}]` — scrolling tothe previous element inside "
-            "an element, with the specified `id`.</p><p>Theoptional "
-            "`overflow` parameter is used to set navigation when the "
-            "first or lastelement is reached:`clamp` — transition will "
-            "stop at the border element;`ring` —go to the beginning or "
-            "end, depending on the current element.</p><p>By "
-            "default,`clamp`."
+            "Action when long-clicking an element. Doesn\'t work on "
+            "devices that don\'t supporttouch gestures."
         ),
     )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
-    orientation: typing.Optional[DivGalleryOrientation] = Field(
-        description="Gallery orientation.",
-    )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    restrict_parent_scroll: typing.Optional[bool] = Field(
-        description=(
-            "If the parameter is enabled, the gallery won\'t transmit "
-            "the scroll gesture to theparent element."
-        ),
-    )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    scroll_mode: typing.Optional[DivGalleryScrollMode] = Field(
-        description=(
-            "Scroll type: `default` — continuous, `paging` — "
-            "page-by-page."
-        ),
-    )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -274,49 +240,72 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-class DivGalleryCrossContentAlignment(str, enum.Enum):
-    START = "start"
-    CENTER = "center"
-    END = "end"
+# Separator display settings.
+class DivSeparatorDelimiterStyle(BaseDiv):
 
+    def __init__(
+        self, *,
+        color: typing.Optional[typing.Union[Expr, str]] = None,
+        orientation: typing.Optional[typing.Union[Expr, DelimiterStyleOrientation]] = None,
+        **kwargs: typing.Any,
+    ):
+        super().__init__(
+            color=color,
+            orientation=orientation,
+            **kwargs,
+        )
 
-class DivGalleryOrientation(str, enum.Enum):
-    HORIZONTAL = "horizontal"
+    color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description=(
+            "Separator color. To prevent the separator from being "
+            "displayed, set transparencyin the alpha channel. For "
+            "example, `#00FFFFFF`."
+        ),
+    )
+    orientation: typing.Optional[typing.Union[Expr, DelimiterStyleOrientation]] = Field(
+        description=(
+            "Separator orientation:`vertical` — vertical;`horizontal` — "
+            "horizontal.<"
+        ),
+    )
+
+
+class DelimiterStyleOrientation(str, enum.Enum):
     VERTICAL = "vertical"
+    HORIZONTAL = "horizontal"
 
 
-class DivGalleryScrollMode(str, enum.Enum):
-    PAGING = "paging"
-    DEFAULT = "default"
+DivSeparatorDelimiterStyle.update_forward_refs()
 
 
-DivGallery.update_forward_refs()
+DivSeparator.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_gif_image.py` & `pydivkit-25.6.0/pydivkit/div/div_select.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,267 +2,253 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
-    div_alignment_vertical, div_animation, div_appearance_transition,
-    div_aspect, div_background, div_border, div_change_transition,
-    div_edge_insets, div_extension, div_focus, div_image_scale, div_size,
-    div_tooltip, div_transform, div_transition_trigger, div_visibility,
-    div_visibility_action,
+    div_alignment_vertical, div_appearance_transition, div_background,
+    div_border, div_change_transition, div_disappear_action, div_edge_insets,
+    div_extension, div_focus, div_font_family, div_font_weight, div_size,
+    div_size_unit, div_tooltip, div_transform, div_transition_trigger,
+    div_visibility, div_visibility_action,
 )
 
 
-# Animated GIF image.
-class DivGifImage(BaseDiv):
+# List of options with only one to be selected.
+class DivSelect(BaseDiv):
 
     def __init__(
         self, *,
-        gif_url: str,
-        type: str = "gif",
+        type: str = "select",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        action: typing.Optional[div_action.DivAction] = None,
-        action_animation: typing.Optional[div_animation.DivAnimation] = None,
-        actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        aspect: typing.Optional[div_aspect.DivAspect] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        doubletap_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
+        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_size: typing.Optional[typing.Union[Expr, int]] = None,
+        font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
-        longtap_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
+        hint_color: typing.Optional[typing.Union[Expr, str]] = None,
+        hint_text: typing.Optional[typing.Union[Expr, str]] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        letter_spacing: typing.Optional[typing.Union[Expr, float]] = None,
+        line_height: typing.Optional[typing.Union[Expr, int]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
+        options: typing.Optional[typing.Sequence[DivSelectOption]] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        placeholder_color: typing.Optional[str] = None,
-        preload_required: typing.Optional[bool] = None,
-        preview: typing.Optional[str] = None,
-        row_span: typing.Optional[int] = None,
-        scale: typing.Optional[div_image_scale.DivImageScale] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        text_color: typing.Optional[typing.Union[Expr, str]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        value_variable: typing.Optional[typing.Union[Expr, str]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
-            action=action,
-            action_animation=action_animation,
-            actions=actions,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
-            aspect=aspect,
             background=background,
             border=border,
             column_span=column_span,
-            content_alignment_horizontal=content_alignment_horizontal,
-            content_alignment_vertical=content_alignment_vertical,
-            doubletap_actions=doubletap_actions,
+            disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
-            gif_url=gif_url,
+            font_family=font_family,
+            font_size=font_size,
+            font_size_unit=font_size_unit,
+            font_weight=font_weight,
             height=height,
+            hint_color=hint_color,
+            hint_text=hint_text,
             id=id,
-            longtap_actions=longtap_actions,
+            letter_spacing=letter_spacing,
+            line_height=line_height,
             margins=margins,
+            options=options,
             paddings=paddings,
-            placeholder_color=placeholder_color,
-            preload_required=preload_required,
-            preview=preview,
             row_span=row_span,
-            scale=scale,
             selected_actions=selected_actions,
+            text_color=text_color,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
+            value_variable=value_variable,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="gif")
+    type: str = Field(default="select")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    action: typing.Optional[div_action.DivAction] = Field(
-        description=(
-            "One action when clicking on an element. Not used if the "
-            "`actions` parameter isset."
-        ),
-    )
-    action_animation: typing.Optional[div_animation.DivAnimation] = Field(
-        description=(
-            "Action animation. Web supports `fade`, `scale` and `set` "
-            "only."
-        ),
-    )
-    actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
-        min_items=1, 
-        description="Multiple actions when clicking on an element.",
-    )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    aspect: typing.Optional[div_aspect.DivAspect] = Field(
-    )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
-        description="Horizontal image alignment.",
-    )
-    content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
-        description="Vertical image alignment.",
-    )
-    doubletap_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         min_items=1, 
-        description="Action when double-clicking on an element.",
+        description="Actions when an element disappears from the screen.",
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
-    gif_url: str = Field(
-        format="uri", 
-        description="Direct URL to a GIF image.",
+    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
+        description=(
+            "Font family:`text` — a standard text font;`display` — a "
+            "family of fonts with alarge font size."
+        ),
+    )
+    font_size: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Font size.",
+    )
+    font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
+        description=(
+            "Unit of measurement:`px` — a physical pixel.`dp` — a "
+            "logical pixel that doesn\'tdepend on screen density.`sp` — "
+            "a logical pixel that depends on the font size ona device. "
+            "Specify height in `sp`. Only available on Android."
+        ),
+    )
+    font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = Field(
+        description="Style.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    hint_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Hint color.",
+    )
+    hint_text: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
+        description="Hint text.",
+    )
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    longtap_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
-        min_items=1, 
+    letter_spacing: typing.Optional[typing.Union[Expr, float]] = Field(
+        description="Spacing between characters.",
+    )
+    line_height: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
-            "Action when long-clicking on an element. Doesn\'t work on "
-            "the devices w/o touchgestures."
+            "Line spacing of the text. Measured in units set in "
+            "`font_size_unit`."
         ),
     )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
+    options: typing.Sequence[DivSelectOption] = Field(
+        min_items=1,
+    )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    placeholder_color: typing.Optional[str] = Field(
-        format="color", 
-        description="Placeholder background before the image is loaded.",
-    )
-    preload_required: typing.Optional[bool] = Field(
-        description="Background image must be loaded before the display.",
-    )
-    preview: typing.Optional[str] = Field(
-        min_length=1, 
-        description=(
-            "Image preview encoded in `base64`. It will be shown instead "
-            "of`placeholder_color` before the image is loaded. Format "
-            "`data url`:`data:[;base64],<data>`"
-        ),
-    )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    scale: typing.Optional[div_image_scale.DivImageScale] = Field(
-        description=(
-            "Image scaling:`fit` places the entire image into the "
-            "element (free space isfilled with background);`fill` scales "
-            "the image to the element size and cuts offthe excess."
-        ),
-    )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    text_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Text color.",
+    )
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -278,33 +264,69 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    value_variable: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description=(
+            "Name of the variable that stores the selected option value "
+            "(`value`)."
+        ),
+    )
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-DivGifImage.update_forward_refs()
+# List option.
+class DivSelectOption(BaseDiv):
+
+    def __init__(
+        self, *,
+        text: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
+    ):
+        super().__init__(
+            text=text,
+            value=value,
+            **kwargs,
+        )
+
+    text: typing.Optional[typing.Union[Expr, str]] = Field(
+        description=(
+            "Text description of the option displayed in the list. If "
+            "not set, `value` is usedinstead."
+        ),
+    )
+    value: typing.Union[Expr, str] = Field(
+        description="Value matching the option.",
+    )
+
+
+DivSelectOption.update_forward_refs()
+
+
+DivSelect.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_image.py` & `pydivkit-25.6.0/pydivkit/div/div_slider.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,187 +2,156 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
-    div_alignment_vertical, div_animation, div_appearance_transition,
-    div_aspect, div_background, div_blend_mode, div_border,
-    div_change_transition, div_edge_insets, div_extension, div_fade_transition,
-    div_focus, div_image_scale, div_size, div_tooltip, div_transform,
-    div_transition_trigger, div_visibility, div_visibility_action,
+    div_alignment_vertical, div_appearance_transition, div_background,
+    div_border, div_change_transition, div_disappear_action, div_drawable,
+    div_edge_insets, div_extension, div_focus, div_font_weight, div_point,
+    div_size, div_size_unit, div_tooltip, div_transform, div_transition_trigger,
+    div_visibility, div_visibility_action,
 )
 
 
-# Image.
-class DivImage(BaseDiv):
+# Slider for selecting a value in the range.
+class DivSlider(BaseDiv):
 
     def __init__(
         self, *,
-        image_url: str,
-        type: str = "image",
+        type: str = "slider",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        action: typing.Optional[div_action.DivAction] = None,
-        action_animation: typing.Optional[div_animation.DivAnimation] = None,
-        actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        appearance_animation: typing.Optional[div_fade_transition.DivFadeTransition] = None,
-        aspect: typing.Optional[div_aspect.DivAspect] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        doubletap_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        high_priority_preview_show: typing.Optional[bool] = None,
-        id: typing.Optional[str] = None,
-        longtap_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
+        max_value: typing.Optional[typing.Union[Expr, int]] = None,
+        min_value: typing.Optional[typing.Union[Expr, int]] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        placeholder_color: typing.Optional[str] = None,
-        preload_required: typing.Optional[bool] = None,
-        preview: typing.Optional[str] = None,
-        row_span: typing.Optional[int] = None,
-        scale: typing.Optional[div_image_scale.DivImageScale] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        tint_color: typing.Optional[str] = None,
-        tint_mode: typing.Optional[div_blend_mode.DivBlendMode] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        secondary_value_accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        thumb_secondary_style: typing.Optional[div_drawable.DivDrawable] = None,
+        thumb_secondary_text_style: typing.Optional[DivSliderTextStyle] = None,
+        thumb_secondary_value_variable: typing.Optional[typing.Union[Expr, str]] = None,
+        thumb_style: typing.Optional[div_drawable.DivDrawable] = None,
+        thumb_text_style: typing.Optional[DivSliderTextStyle] = None,
+        thumb_value_variable: typing.Optional[typing.Union[Expr, str]] = None,
+        tick_mark_active_style: typing.Optional[div_drawable.DivDrawable] = None,
+        tick_mark_inactive_style: typing.Optional[div_drawable.DivDrawable] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
+        track_active_style: typing.Optional[div_drawable.DivDrawable] = None,
+        track_inactive_style: typing.Optional[div_drawable.DivDrawable] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
-            action=action,
-            action_animation=action_animation,
-            actions=actions,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
-            appearance_animation=appearance_animation,
-            aspect=aspect,
             background=background,
             border=border,
             column_span=column_span,
-            content_alignment_horizontal=content_alignment_horizontal,
-            content_alignment_vertical=content_alignment_vertical,
-            doubletap_actions=doubletap_actions,
+            disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
             height=height,
-            high_priority_preview_show=high_priority_preview_show,
             id=id,
-            image_url=image_url,
-            longtap_actions=longtap_actions,
             margins=margins,
+            max_value=max_value,
+            min_value=min_value,
             paddings=paddings,
-            placeholder_color=placeholder_color,
-            preload_required=preload_required,
-            preview=preview,
             row_span=row_span,
-            scale=scale,
+            secondary_value_accessibility=secondary_value_accessibility,
             selected_actions=selected_actions,
-            tint_color=tint_color,
-            tint_mode=tint_mode,
+            thumb_secondary_style=thumb_secondary_style,
+            thumb_secondary_text_style=thumb_secondary_text_style,
+            thumb_secondary_value_variable=thumb_secondary_value_variable,
+            thumb_style=thumb_style,
+            thumb_text_style=thumb_text_style,
+            thumb_value_variable=thumb_value_variable,
+            tick_mark_active_style=tick_mark_active_style,
+            tick_mark_inactive_style=tick_mark_inactive_style,
             tooltips=tooltips,
+            track_active_style=track_active_style,
+            track_inactive_style=track_inactive_style,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="image")
+    type: str = Field(default="slider")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    action: typing.Optional[div_action.DivAction] = Field(
-        description=(
-            "One action when clicking on an element. Not used if the "
-            "`actions` parameter isset."
-        ),
-    )
-    action_animation: typing.Optional[div_animation.DivAnimation] = Field(
-        description=(
-            "Action animation. Web supports `fade`, `scale` and `set` "
-            "only."
-        ),
-    )
-    actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
-        min_items=1, 
-        description="Multiple actions when clicking on an element.",
-    )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    appearance_animation: typing.Optional[div_fade_transition.DivFadeTransition] = Field(
-        description="Transparency animation when loading an image.",
-    )
-    aspect: typing.Optional[div_aspect.DivAspect] = Field(
-    )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
-        description="Horizontal image alignment.",
-    )
-    content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
-        description="Vertical image alignment.",
-    )
-    doubletap_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
         min_items=1, 
-        description="Action when double-clicking on an element.",
+        description="Actions when an element disappears from the screen.",
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
@@ -194,102 +163,98 @@
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    high_priority_preview_show: typing.Optional[bool] = Field(
-        description=(
-            "It sets the priority of displaying the preview — the "
-            "preview is decoded in themain stream and displayed as the "
-            "first frame. Use the parameter carefully — itwill worsen "
-            "the preview display time and can worsen the application "
-            "launch time."
-        ),
-    )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    image_url: str = Field(
-        format="uri", 
-        description="Direct URL to an image.",
-    )
-    longtap_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
-        min_items=1, 
-        description=(
-            "Action when long-clicking on an element. Doesn\'t work on "
-            "the devices w/o touchgestures."
-        ),
-    )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
-    paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
-        description="Internal margins from the element stroke.",
-    )
-    placeholder_color: typing.Optional[str] = Field(
-        format="color", 
-        description="Placeholder background before the image is loaded.",
+    max_value: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Maximum value. It must be greater than the minimum value.",
     )
-    preload_required: typing.Optional[bool] = Field(
-        description="Background image must be loaded before the display.",
+    min_value: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Minimum value.",
     )
-    preview: typing.Optional[str] = Field(
-        min_length=1, 
-        description=(
-            "Image preview encoded in `base64`. It will be shown instead "
-            "of`placeholder_color` before the image is loaded. Format "
-            "`data url`:`data:[;base64],<data>`"
-        ),
+    paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
+        description="Internal margins from the element stroke.",
     )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    scale: typing.Optional[div_image_scale.DivImageScale] = Field(
-        description=(
-            "Image scaling:`fit` places the entire image into the "
-            "element (free space isfilled with background);`fill` scales "
-            "the image to the element size and cuts offthe excess."
-        ),
+    secondary_value_accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
+        description="Accessibility settings for the second pointer.",
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    tint_color: typing.Optional[str] = Field(
-        format="color", 
-        description="New color of a contour image.",
+    thumb_secondary_style: typing.Optional[div_drawable.DivDrawable] = Field(
+        description="Style of the second pointer.",
     )
-    tint_mode: typing.Optional[div_blend_mode.DivBlendMode] = Field(
-        description="The blend mode of color specified in tint_color.",
+    thumb_secondary_text_style: typing.Optional[DivSliderTextStyle] = Field(
+        description="Text style in the second pointer.",
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    thumb_secondary_value_variable: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
+        description=(
+            "Name of the variable to store the second pointer\'s current "
+            "value."
+        ),
+    )
+    thumb_style: div_drawable.DivDrawable = Field(
+        description="Style of the first pointer.",
+    )
+    thumb_text_style: typing.Optional[DivSliderTextStyle] = Field(
+        description="Text style in the first pointer.",
+    )
+    thumb_value_variable: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
+        description=(
+            "Name of the variable to store the pointer\'s current value."
+        ),
+    )
+    tick_mark_active_style: typing.Optional[div_drawable.DivDrawable] = Field(
+        description="Style of active serifs.",
+    )
+    tick_mark_inactive_style: typing.Optional[div_drawable.DivDrawable] = Field(
+        description="Style of inactive serifs.",
+    )
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
+    track_active_style: div_drawable.DivDrawable = Field(
+        description="Style of the active part of a scale.",
+    )
+    track_inactive_style: div_drawable.DivDrawable = Field(
+        description="Style of the inactive part of a scale.",
+    )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -305,33 +270,73 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-DivImage.update_forward_refs()
+class DivSliderTextStyle(BaseDiv):
+
+    def __init__(
+        self, *,
+        font_size: typing.Optional[typing.Union[Expr, int]] = None,
+        font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
+        offset: typing.Optional[div_point.DivPoint] = None,
+        text_color: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
+    ):
+        super().__init__(
+            font_size=font_size,
+            font_size_unit=font_size_unit,
+            font_weight=font_weight,
+            offset=offset,
+            text_color=text_color,
+            **kwargs,
+        )
+
+    font_size: typing.Union[Expr, int] = Field(
+        description="Font size.",
+    )
+    font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
+    )
+    font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = Field(
+        description="Style.",
+    )
+    offset: typing.Optional[div_point.DivPoint] = Field(
+        description="Shift relative to the center.",
+    )
+    text_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Text color.",
+    )
+
+
+DivSliderTextStyle.update_forward_refs()
+
+
+DivSlider.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_image_background.py` & `pydivkit-25.6.0/pydivkit/div/div_image_background.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,58 +2,69 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_alignment_horizontal, div_alignment_vertical, div_image_scale
+from . import (
+    div_alignment_horizontal, div_alignment_vertical, div_filter,
+    div_image_scale,
+)
 
 
 # Background image.
 class DivImageBackground(BaseDiv):
 
     def __init__(
         self, *,
-        image_url: str,
         type: str = "image",
-        alpha: typing.Optional[float] = None,
-        content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        preload_required: typing.Optional[bool] = None,
-        scale: typing.Optional[div_image_scale.DivImageScale] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        filters: typing.Optional[typing.Sequence[div_filter.DivFilter]] = None,
+        image_url: typing.Optional[typing.Union[Expr, str]] = None,
+        preload_required: typing.Optional[typing.Union[Expr, bool]] = None,
+        scale: typing.Optional[typing.Union[Expr, div_image_scale.DivImageScale]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             alpha=alpha,
             content_alignment_horizontal=content_alignment_horizontal,
             content_alignment_vertical=content_alignment_vertical,
+            filters=filters,
             image_url=image_url,
             preload_required=preload_required,
             scale=scale,
+            **kwargs,
         )
 
     type: str = Field(default="image")
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description="Image transparency.",
     )
-    content_alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description="Horizontal image alignment.",
     )
-    content_alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description="Vertical image alignment.",
     )
-    image_url: str = Field(
+    filters: typing.Optional[typing.Sequence[div_filter.DivFilter]] = Field(
+        min_items=1, 
+        description="Image filters.",
+    )
+    image_url: typing.Union[Expr, str] = Field(
         format="uri", 
         description="Image URL.",
     )
-    preload_required: typing.Optional[bool] = Field(
+    preload_required: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="Background image must be loaded before the display.",
     )
-    scale: typing.Optional[div_image_scale.DivImageScale] = Field(
+    scale: typing.Optional[typing.Union[Expr, div_image_scale.DivImageScale]] = Field(
         description="Image scaling.",
     )
 
 
 DivImageBackground.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_indicator.py` & `pydivkit-25.6.0/pydivkit/div/div_video.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,224 +2,264 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_edge_insets, div_extension,
-    div_fixed_size, div_focus, div_shape, div_size, div_tooltip, div_transform,
-    div_transition_trigger, div_visibility, div_visibility_action,
+    div_border, div_change_transition, div_disappear_action, div_edge_insets,
+    div_extension, div_focus, div_size, div_tooltip, div_transform,
+    div_transition_trigger, div_video_source, div_visibility,
+    div_visibility_action,
 )
 
 
-# Progress indicator for [pager](div-pager.md).
-class DivIndicator(BaseDiv):
+# Video.
+class DivVideo(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "indicator",
+        type: str = "video",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        active_item_color: typing.Optional[str] = None,
-        active_item_size: typing.Optional[float] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        animation: typing.Optional[DivIndicatorAnimation] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        autostart: typing.Optional[typing.Union[Expr, bool]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        buffering_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        elapsed_time_variable: typing.Optional[typing.Union[Expr, str]] = None,
+        end_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
+        fatal_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
-        inactive_item_color: typing.Optional[str] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        minimum_item_size: typing.Optional[float] = None,
+        muted: typing.Optional[typing.Union[Expr, bool]] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        pager_id: typing.Optional[str] = None,
-        row_span: typing.Optional[int] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        shape: typing.Optional[div_shape.DivShape] = None,
-        space_between_centers: typing.Optional[div_fixed_size.DivFixedSize] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        pause_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        player_settings_payload: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        preview: typing.Optional[typing.Union[Expr, str]] = None,
+        repeatable: typing.Optional[typing.Union[Expr, bool]] = None,
+        resume_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        video_sources: typing.Optional[typing.Sequence[div_video_source.DivVideoSource]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
-            active_item_color=active_item_color,
-            active_item_size=active_item_size,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
-            animation=animation,
+            autostart=autostart,
             background=background,
             border=border,
+            buffering_actions=buffering_actions,
             column_span=column_span,
+            disappear_actions=disappear_actions,
+            elapsed_time_variable=elapsed_time_variable,
+            end_actions=end_actions,
             extensions=extensions,
+            fatal_actions=fatal_actions,
             focus=focus,
             height=height,
             id=id,
-            inactive_item_color=inactive_item_color,
             margins=margins,
-            minimum_item_size=minimum_item_size,
+            muted=muted,
             paddings=paddings,
-            pager_id=pager_id,
+            pause_actions=pause_actions,
+            player_settings_payload=player_settings_payload,
+            preview=preview,
+            repeatable=repeatable,
+            resume_actions=resume_actions,
             row_span=row_span,
             selected_actions=selected_actions,
-            shape=shape,
-            space_between_centers=space_between_centers,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
+            video_sources=video_sources,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="indicator")
+    type: str = Field(default="video")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    active_item_color: typing.Optional[str] = Field(
-        format="color", 
-        description="Active indicator color.",
-    )
-    active_item_size: typing.Optional[float] = Field(
-        description="A size multiplier for an active indicator.",
-    )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    animation: typing.Optional[DivIndicatorAnimation] = Field(
-        description="Animation of switching between indicators.",
+    autostart: typing.Optional[typing.Union[Expr, bool]] = Field(
+        description=(
+            "This option turns on automatic video playback. On the web, "
+            "the video starts ifmuted playback is turned on."
+        ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    buffering_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Actions performed during video loading.",
+    )
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    elapsed_time_variable: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
+        description=(
+            "Time interval from the video beginning to the current "
+            "position in milliseconds."
+        ),
+    )
+    end_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Actions performed after the video ends.",
+    )
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
+    fatal_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description=(
+            "Actions that are performed when it is impossible to "
+            "continue playback due to anerror in the player."
+        ),
+    )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    inactive_item_color: typing.Optional[str] = Field(
-        format="color", 
-        description="Indicator color.",
-    )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
-    minimum_item_size: typing.Optional[float] = Field(
-        description=(
-            "A size multiplier for a minimal indicator. It is used when "
-            "the required number ofindicators don\'t fit on the screen."
-        ),
+    muted: typing.Optional[typing.Union[Expr, bool]] = Field(
+        description="This option mutes video.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    pager_id: typing.Optional[str] = Field(
-        description="ID of the pager that is a data source for an indicator.",
+    pause_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Actions that are performed when a playback is paused.",
+    )
+    player_settings_payload: typing.Optional[typing.Dict[str, typing.Any]] = Field(
+        description="Additional information that can be used in the player.",
     )
-    row_span: typing.Optional[int] = Field(
+    preview: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
+        description=(
+            "Video preview encoded in `base64`. Will be shown until the "
+            "video is ready toplay. `Data url` format: "
+            "`data:[;base64],<data>`"
+        ),
+    )
+    repeatable: typing.Optional[typing.Union[Expr, bool]] = Field(
+        description="This option turns on video repeat.",
+    )
+    resume_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Actions performed when video playback resumes.",
+    )
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    shape: typing.Optional[div_shape.DivShape] = Field(
-        description="Indicator shape.",
-    )
-    space_between_centers: typing.Optional[div_fixed_size.DivFixedSize] = Field(
-        description="Spacing between indicator centers.",
-    )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -235,39 +275,36 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    video_sources: typing.Sequence[div_video_source.DivVideoSource] = Field(
+        min_items=1,
+    )
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-class DivIndicatorAnimation(str, enum.Enum):
-    SCALE = "scale"
-    WORM = "worm"
-    SLIDER = "slider"
-
-
-DivIndicator.update_forward_refs()
+DivVideo.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_input.py` & `pydivkit-25.6.0/pydivkit/div/div_input.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,82 +2,87 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_edge_insets, div_extension,
-    div_focus, div_font_family, div_font_weight, div_size, div_size_unit,
-    div_tooltip, div_transform, div_transition_trigger, div_visibility,
-    div_visibility_action,
+    div_border, div_change_transition, div_disappear_action, div_edge_insets,
+    div_extension, div_focus, div_font_family, div_font_weight, div_input_mask,
+    div_input_validator, div_size, div_size_unit, div_tooltip, div_transform,
+    div_transition_trigger, div_visibility, div_visibility_action,
 )
 
 
 # Text input element.
 class DivInput(BaseDiv):
 
     def __init__(
         self, *,
-        text_variable: str,
         type: str = "input",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
-        font_family: typing.Optional[div_font_family.DivFontFamily] = None,
-        font_size: typing.Optional[int] = None,
-        font_size_unit: typing.Optional[div_size_unit.DivSizeUnit] = None,
-        font_weight: typing.Optional[div_font_weight.DivFontWeight] = None,
+        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_size: typing.Optional[typing.Union[Expr, int]] = None,
+        font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        highlight_color: typing.Optional[str] = None,
-        hint_color: typing.Optional[str] = None,
-        hint_text: typing.Optional[str] = None,
-        id: typing.Optional[str] = None,
-        keyboard_type: typing.Optional[DivInputKeyboardType] = None,
-        letter_spacing: typing.Optional[float] = None,
-        line_height: typing.Optional[int] = None,
+        highlight_color: typing.Optional[typing.Union[Expr, str]] = None,
+        hint_color: typing.Optional[typing.Union[Expr, str]] = None,
+        hint_text: typing.Optional[typing.Union[Expr, str]] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        keyboard_type: typing.Optional[typing.Union[Expr, DivInputKeyboardType]] = None,
+        letter_spacing: typing.Optional[typing.Union[Expr, float]] = None,
+        line_height: typing.Optional[typing.Union[Expr, int]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        max_visible_lines: typing.Optional[int] = None,
+        mask: typing.Optional[div_input_mask.DivInputMask] = None,
+        max_visible_lines: typing.Optional[typing.Union[Expr, int]] = None,
         native_interface: typing.Optional[DivInputNativeInterface] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        row_span: typing.Optional[int] = None,
-        select_all_on_focus: typing.Optional[bool] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        text_color: typing.Optional[str] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        select_all_on_focus: typing.Optional[typing.Union[Expr, bool]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        text_color: typing.Optional[typing.Union[Expr, str]] = None,
+        text_variable: typing.Optional[typing.Union[Expr, str]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        validators: typing.Optional[typing.Sequence[div_input_validator.DivInputValidator]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
             background=background,
             border=border,
             column_span=column_span,
+            disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
             font_family=font_family,
             font_size=font_size,
             font_size_unit=font_size_unit,
             font_weight=font_weight,
             height=height,
@@ -85,195 +90,202 @@
             hint_color=hint_color,
             hint_text=hint_text,
             id=id,
             keyboard_type=keyboard_type,
             letter_spacing=letter_spacing,
             line_height=line_height,
             margins=margins,
+            mask=mask,
             max_visible_lines=max_visible_lines,
             native_interface=native_interface,
             paddings=paddings,
             row_span=row_span,
             select_all_on_focus=select_all_on_focus,
             selected_actions=selected_actions,
             text_color=text_color,
             text_variable=text_variable,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
+            validators=validators,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
     type: str = Field(default="input")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
-    font_family: typing.Optional[div_font_family.DivFontFamily] = Field(
+    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
         description=(
             "Font family:`text` — a standard text font;`display` — a "
             "family of fonts with alarge font size."
         ),
     )
-    font_size: typing.Optional[int] = Field(
+    font_size: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Font size.",
     )
-    font_size_unit: typing.Optional[div_size_unit.DivSizeUnit] = Field(
+    font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description=(
             "Unit of measurement:`px` — a physical pixel.`dp` — a "
             "logical pixel that doesn\'tdepend on screen density.`sp` — "
             "a logical pixel that depends on the font size ona device. "
             "Specify height in `sp`. Only available on Android."
         ),
     )
-    font_weight: typing.Optional[div_font_weight.DivFontWeight] = Field(
+    font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = Field(
         description="Style.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    highlight_color: typing.Optional[str] = Field(
+    highlight_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description=(
             "Text highlight color. If the value isn\'t set, the color "
             "set in the client will beused instead."
         ),
     )
-    hint_color: typing.Optional[str] = Field(
+    hint_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Text color.",
     )
-    hint_text: typing.Optional[str] = Field(
+    hint_text: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description="Tooltip text.",
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    keyboard_type: typing.Optional[DivInputKeyboardType] = Field(
+    keyboard_type: typing.Optional[typing.Union[Expr, DivInputKeyboardType]] = Field(
         description="Keyboard type.",
     )
-    letter_spacing: typing.Optional[float] = Field(
+    letter_spacing: typing.Optional[typing.Union[Expr, float]] = Field(
         description="Spacing between characters.",
     )
-    line_height: typing.Optional[int] = Field(
+    line_height: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
-            "Line spacing of the text range. The count is taken from the "
-            "font baseline.Measured in units specified in "
+            "Line spacing of the text. Units specified in "
             "`font_size_unit`."
         ),
     )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
-    max_visible_lines: typing.Optional[int] = Field(
+    mask: typing.Optional[div_input_mask.DivInputMask] = Field(
+        description="Mask for entering text based on the specified template.",
+    )
+    max_visible_lines: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
-            "Maximum number of lines that will be visible in the input "
-            "view."
+            "Maximum number of lines to be displayed in the input field."
         ),
     )
     native_interface: typing.Optional[DivInputNativeInterface] = Field(
         description="Text input line used in the native interface.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    select_all_on_focus: typing.Optional[bool] = Field(
+    select_all_on_focus: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="Highlighting input text when focused.",
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    text_color: typing.Optional[str] = Field(
+    text_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Text color.",
     )
-    text_variable: str = Field(
+    text_variable: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Name of text storage variable.",
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -289,31 +301,35 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    validators: typing.Optional[typing.Sequence[div_input_validator.DivInputValidator]] = Field(
+        min_items=1, 
+        description="Validators for text value.",
+    )
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
@@ -328,21 +344,23 @@
 
 
 # Text input line used in the native interface.
 class DivInputNativeInterface(BaseDiv):
 
     def __init__(
         self, *,
-        color: str,
+        color: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             color=color,
+            **kwargs,
         )
 
-    color: str = Field(
+    color: typing.Union[Expr, str] = Field(
         format="color", 
         description="Text input line color.",
     )
 
 
 DivInputNativeInterface.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_linear_gradient.py` & `pydivkit-25.6.0/pydivkit/div/div_linear_gradient.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
 # Linear gradient.
 class DivLinearGradient(BaseDiv):
 
     def __init__(
         self, *,
-        colors: typing.List[str],
         type: str = "gradient",
-        angle: typing.Optional[int] = None,
+        angle: typing.Optional[typing.Union[Expr, int]] = None,
+        colors: typing.Optional[typing.Sequence[typing.Union[Expr, str]]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             angle=angle,
             colors=colors,
+            **kwargs,
         )
 
     type: str = Field(default="gradient")
-    angle: typing.Optional[int] = Field(
+    angle: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Angle of gradient direction.",
     )
-    colors: typing.List[str] = Field(
+    colors: typing.Sequence[typing.Union[Expr, str]] = Field(
         min_items=2, 
         description=(
-            "Colors. Gradient points will be located at an equal "
-            "distance from each other."
+            "Colors. Gradient points are located at an equal distance "
+            "from each other."
         ),
     )
 
 
 DivLinearGradient.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_match_parent_size.py` & `pydivkit-25.6.0/pydivkit/div/div_match_parent_size.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
 # Element size adjusts to a parent element.
 class DivMatchParentSize(BaseDiv):
 
     def __init__(
         self, *,
         type: str = "match_parent",
-        weight: typing.Optional[float] = None,
+        weight: typing.Optional[typing.Union[Expr, float]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             weight=weight,
+            **kwargs,
         )
 
     type: str = Field(default="match_parent")
-    weight: typing.Optional[float] = Field(
+    weight: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Weight when distributing free space between elements with "
             "the size type`match_parent` inside an element. If the "
             "weight isn\'t specified, the elementswill divide the place "
             "equally."
         ),
     )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_neighbour_page_size.py` & `pydivkit-25.6.0/pydivkit/div/div_neighbour_page_size.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_fixed_size
 
 
 # Fixed width value of the visible part of a neighbouring page.
 class DivNeighbourPageSize(BaseDiv):
 
     def __init__(
         self, *,
-        neighbour_page_width: div_fixed_size.DivFixedSize,
         type: str = "fixed",
+        neighbour_page_width: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             neighbour_page_width=neighbour_page_width,
+            **kwargs,
         )
 
     type: str = Field(default="fixed")
     neighbour_page_width: div_fixed_size.DivFixedSize = Field(
         description="Width of the visible part of a neighbouring page.",
     )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_page_size.py` & `pydivkit-25.6.0/pydivkit/div/div_pivot_percentage.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_percentage_size
 
-
-# Percentage value of the page width.
-class DivPageSize(BaseDiv):
+# Location of the coordinate of the rotation axis as a percentage relative to the
+# element size.
+class DivPivotPercentage(BaseDiv):
 
     def __init__(
         self, *,
-        page_width: div_percentage_size.DivPercentageSize,
-        type: str = "percentage",
+        type: str = "pivot-percentage",
+        value: typing.Optional[typing.Union[Expr, float]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            page_width=page_width,
+            value=value,
+            **kwargs,
         )
 
-    type: str = Field(default="percentage")
-    page_width: div_percentage_size.DivPercentageSize = Field(
-        description="Page width as a percentage of the parent element width.",
+    type: str = Field(default="pivot-percentage")
+    value: typing.Union[Expr, float] = Field(
+        description="Coordinate value as a percentage.",
     )
 
 
-DivPageSize.update_forward_refs()
+DivPivotPercentage.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_pager.py` & `pydivkit-25.6.0/pydivkit/div/div_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,141 +2,151 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
-    div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_edge_insets, div_extension,
-    div_fixed_size, div_focus, div_pager_layout_mode, div_size, div_tooltip,
-    div_transform, div_transition_trigger, div_visibility,
-    div_visibility_action,
+    div_alignment_vertical, div_animation, div_appearance_transition,
+    div_background, div_border, div_change_transition, div_disappear_action,
+    div_edge_insets, div_extension, div_focus, div_size, div_tooltip,
+    div_transform, div_transition_selector, div_transition_trigger,
+    div_visibility, div_visibility_action,
 )
 
 
-# Pager. It contains a horizontal set of cards that can be scrolled page by page.
-# It shows the main page and the beginning of the next one.
-class DivPager(BaseDiv):
+# It contains sets of states for visual elements and switches between them.
+class DivState(BaseDiv):
 
     def __init__(
         self, *,
-        items: typing.List[div.Div],
-        layout_mode: div_pager_layout_mode.DivPagerLayoutMode,
-        type: str = "pager",
+        type: str = "state",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        default_item: typing.Optional[int] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        default_state_id: typing.Optional[typing.Union[Expr, str]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        div_id: typing.Optional[typing.Union[Expr, str]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
-        item_spacing: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        orientation: typing.Optional[DivPagerOrientation] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        restrict_parent_scroll: typing.Optional[bool] = None,
-        row_span: typing.Optional[int] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        states: typing.Optional[typing.Sequence[DivStateState]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
+        transition_animation_selector: typing.Optional[typing.Union[Expr, div_transition_selector.DivTransitionSelector]] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
             background=background,
             border=border,
             column_span=column_span,
-            default_item=default_item,
+            default_state_id=default_state_id,
+            disappear_actions=disappear_actions,
+            div_id=div_id,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
-            item_spacing=item_spacing,
-            items=items,
-            layout_mode=layout_mode,
             margins=margins,
-            orientation=orientation,
             paddings=paddings,
-            restrict_parent_scroll=restrict_parent_scroll,
             row_span=row_span,
             selected_actions=selected_actions,
+            states=states,
             tooltips=tooltips,
             transform=transform,
+            transition_animation_selector=transition_animation_selector,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="pager")
+    type: str = Field(default="state")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    default_item: typing.Optional[int] = Field(
+    default_state_id: typing.Optional[typing.Union[Expr, str]] = Field(
         description=(
-            "Ordinal number of the pager element that will be opened by "
-            "default."
+            "ID of the status that will be set by default. If the "
+            "parameter isnt set, thefirst state of the `states` will be "
+            "set."
         ),
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    div_id: typing.Optional[typing.Union[Expr, str]] = Field(
+        description=(
+            "ID of an element to search in the hierarchy. The ID must be "
+            "unique at onehierarchy level. @deprecated"
+        ),
+    )
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
@@ -148,93 +158,67 @@
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    item_spacing: typing.Optional[div_fixed_size.DivFixedSize] = Field(
-        description="Spacing between elements.",
-    )
-    items: typing.List[div.Div] = Field(
-        min_items=1, 
-        description=(
-            "Pager elements. Page-by-page transition options can be "
-            "implementedusing:`div-action://set_current_item?id=&item=` "
-            "— set the current page with anordinal number `item` inside "
-            "an element, with the "
-            "specified`id`;`div-action://set_next_item?id=[&overflow={cl"
-            "amp|ring}]` — go to the nextpage inside an element, with "
-            "the "
-            "specified`id`;`div-action://set_previous_item?id=[&overflow"
-            "={clamp|ring}]` — go to theprevious page inside an element, "
-            "with the specified `id`.</p><p>The optional`overflow` "
-            "parameter is used to set navigation when the first or last "
-            "element isreached:`clamp` — transition will stop at the "
-            "border element;`ring` — go to thebeginning or end, "
-            "depending on the current element.</p><p>By default, "
-            "`clamp`."
-        ),
-    )
-    layout_mode: div_pager_layout_mode.DivPagerLayoutMode = Field(
-        description=(
-            "Type of calculation of the main page width:`fixed` — from "
-            "the fixed width of thenext page "
-            "`neighbour_page_width`;`percentage` — from the percentage "
-            "value`page_width`."
-        ),
-    )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
-    orientation: typing.Optional[DivPagerOrientation] = Field(
-        description="Pager orientation.",
-    )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    restrict_parent_scroll: typing.Optional[bool] = Field(
-        description=(
-            "If the parameter is enabled, the pager won\'t transmit the "
-            "scroll gesture to theparent element."
-        ),
-    )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    states: typing.Sequence[DivStateState] = Field(
+        min_items=1, 
+        description=(
+            "States. Each element can have a few states with a different "
+            "layout. Transitionbetween states is performed using "
+            "[special scheme](../../interaction.dita) of "
+            "the[action](div-action.md) element."
+        ),
+    )
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
+        ),
+    )
+    transition_animation_selector: typing.Optional[typing.Union[Expr, div_transition_selector.DivTransitionSelector]] = Field(
+        description=(
+            "It determines which events trigger transition animations. "
+            "@deprecated"
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -250,38 +234,83 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-class DivPagerOrientation(str, enum.Enum):
-    HORIZONTAL = "horizontal"
-    VERTICAL = "vertical"
+class DivStateState(BaseDiv):
+
+    def __init__(
+        self, *,
+        animation_in: typing.Optional[div_animation.DivAnimation] = None,
+        animation_out: typing.Optional[div_animation.DivAnimation] = None,
+        div: typing.Optional[div.Div] = None,
+        state_id: typing.Optional[typing.Union[Expr, str]] = None,
+        swipe_out_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        **kwargs: typing.Any,
+    ):
+        super().__init__(
+            animation_in=animation_in,
+            animation_out=animation_out,
+            div=div,
+            state_id=state_id,
+            swipe_out_actions=swipe_out_actions,
+            **kwargs,
+        )
+
+    animation_in: typing.Optional[div_animation.DivAnimation] = Field(
+        description=(
+            "State appearance animation. Use `transition_in` instead. "
+            "@deprecated"
+        ),
+    )
+    animation_out: typing.Optional[div_animation.DivAnimation] = Field(
+        description=(
+            "State disappearance animation. Use `transition_out` "
+            "instead. @deprecated"
+        ),
+    )
+    div: typing.Optional[div.Div] = Field(
+        description=(
+            "Contents. If the parameter is missing, the state won\'t be "
+            "displayed."
+        ),
+    )
+    state_id: typing.Union[Expr, str] = Field(
+        description="State ID. It must be unique at one hierarchy level.",
+    )
+    swipe_out_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Actions when swiping the state horizontally. @deprecated",
+    )
+
+
+DivStateState.update_forward_refs()
 
 
-DivPager.update_forward_refs()
+DivState.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_patch.py` & `pydivkit-25.6.0/pydivkit/div/div_shape_drawable.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,72 +2,45 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div
+from . import div_shape, div_stroke
 
 
-# Edits the element.
-class DivPatch(BaseDiv):
+# Drawable of a simple geometric shape.
+class DivShapeDrawable(BaseDiv):
 
     def __init__(
         self, *,
-        changes: typing.List[DivPatchChange],
-        mode: typing.Optional[DivPatchMode] = None,
+        type: str = "shape_drawable",
+        color: typing.Optional[typing.Union[Expr, str]] = None,
+        shape: typing.Optional[div_shape.DivShape] = None,
+        stroke: typing.Optional[div_stroke.DivStroke] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            changes=changes,
-            mode=mode,
+            type=type,
+            color=color,
+            shape=shape,
+            stroke=stroke,
+            **kwargs,
         )
 
-    changes: typing.List[DivPatchChange] = Field(
-        min_items=1, 
-        description="Element changes.",
+    type: str = Field(default="shape_drawable")
+    color: typing.Union[Expr, str] = Field(
+        format="color", 
+        description="Fill color. @deprecated",
     )
-    mode: typing.Optional[DivPatchMode] = Field(
-        description=(
-            "Procedure for applying changes:`transactional` — if an "
-            "error occurs duringapplication of at least one element, the "
-            "changes aren\'t applied.`partial` — allpossible changes are "
-            "applied. If there are errors, they are reported."
-        ),
+    shape: div_shape.DivShape = Field(
+        description="Shape.",
     )
-
-
-class DivPatchMode(str, enum.Enum):
-    TRANSACTIONAL = "transactional"
-    PARTIAL = "partial"
-
-
-class DivPatchChange(BaseDiv):
-
-    def __init__(
-        self, *,
-        id: str,
-        items: typing.Optional[typing.List[div.Div]] = None,
-    ):
-        super().__init__(
-            id=id,
-            items=items,
-        )
-
-    id: str = Field(
-        description="ID of an element to be replaced or removed.",
+    stroke: typing.Optional[div_stroke.DivStroke] = Field(
+        description="Stroke style. @deprecated",
     )
-    items: typing.Optional[typing.List[div.Div]] = Field(
-        min_items=1, 
-        description=(
-            "Elements to be inserted. If the parameter isn\'t specified, "
-            "the element will beremoved."
-        ),
-    )
-
-
-DivPatchChange.update_forward_refs()
 
 
-DivPatch.update_forward_refs()
+DivShapeDrawable.update_forward_refs()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_percentage_size.py` & `pydivkit-25.6.0/pydivkit/div/div_blur.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
-# Percentage value of the element size.
-class DivPercentageSize(BaseDiv):
+# Gaussian image blur.
+class DivBlur(BaseDiv):
 
     def __init__(
         self, *,
-        value: float,
-        type: str = "percentage",
+        type: str = "blur",
+        radius: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            value=value,
+            radius=radius,
+            **kwargs,
         )
 
-    type: str = Field(default="percentage")
-    value: float = Field(
-        description="Element size value.",
+    type: str = Field(default="blur")
+    radius: typing.Union[Expr, int] = Field(
+        description=(
+            "Blur radius. Defines how many pixels blend into each other. "
+            "Specified in: `dp`."
+        ),
     )
 
 
-DivPercentageSize.update_forward_refs()
+DivBlur.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_pivot_fixed.py` & `pydivkit-25.6.0/pydivkit/div/div_circle_shape.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,41 +2,45 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_size_unit
+from . import div_fixed_size, div_stroke
 
 
-# Value of the offset of the coordinates of the axis of rotation.
-class DivPivotFixed(BaseDiv):
+# Circle.
+class DivCircleShape(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "pivot-fixed",
-        unit: typing.Optional[div_size_unit.DivSizeUnit] = None,
-        value: typing.Optional[int] = None,
+        type: str = "circle",
+        background_color: typing.Optional[typing.Union[Expr, str]] = None,
+        radius: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        stroke: typing.Optional[div_stroke.DivStroke] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            unit=unit,
-            value=value,
+            background_color=background_color,
+            radius=radius,
+            stroke=stroke,
+            **kwargs,
         )
 
-    type: str = Field(default="pivot-fixed")
-    unit: typing.Optional[div_size_unit.DivSizeUnit] = Field(
-        description=(
-            "Unit of size measurement. To learn more about units of size "
-            "measurement, see[Layout inside the "
-            "card](../../layout.dita)."
-        ),
+    type: str = Field(default="circle")
+    background_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Fill color.",
     )
-    value: typing.Optional[int] = Field(
-        description="Offset.",
+    radius: typing.Optional[div_fixed_size.DivFixedSize] = Field(
+        description="Radius.",
+    )
+    stroke: typing.Optional[div_stroke.DivStroke] = Field(
+        description="Stroke style.",
     )
 
 
-DivPivotFixed.update_forward_refs()
+DivCircleShape.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_pivot_percentage.py` & `pydivkit-25.6.0/pydivkit/div/div_page_size.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
+from . import div_percentage_size
 
-# Location of the coordinate of the axis of rotation as a percentage relative to
-# the element.
-class DivPivotPercentage(BaseDiv):
+
+# Page width (%).
+class DivPageSize(BaseDiv):
 
     def __init__(
         self, *,
-        value: float,
-        type: str = "pivot-percentage",
+        type: str = "percentage",
+        page_width: typing.Optional[div_percentage_size.DivPercentageSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            value=value,
+            page_width=page_width,
+            **kwargs,
         )
 
-    type: str = Field(default="pivot-percentage")
-    value: float = Field(
-        description="Location of the element.",
+    type: str = Field(default="percentage")
+    page_width: div_percentage_size.DivPercentageSize = Field(
+        description="Page width as a percentage of the parent element width.",
     )
 
 
-DivPivotPercentage.update_forward_refs()
+DivPageSize.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_point.py` & `pydivkit-25.6.0/pydivkit/div/div_stroke.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,34 +2,41 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_dimension
+from . import div_size_unit
 
 
-# A point with fixed coordinates.
-class DivPoint(BaseDiv):
+# Stroke.
+class DivStroke(BaseDiv):
 
     def __init__(
         self, *,
-        x: div_dimension.DivDimension,
-        y: div_dimension.DivDimension,
+        color: typing.Optional[typing.Union[Expr, str]] = None,
+        unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        width: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            x=x,
-            y=y,
+            color=color,
+            unit=unit,
+            width=width,
+            **kwargs,
         )
 
-    x: div_dimension.DivDimension = Field(
-        description="`X` coordinate.",
+    color: typing.Union[Expr, str] = Field(
+        format="color", 
+        description="Stroke color.",
     )
-    y: div_dimension.DivDimension = Field(
-        description="`Y` coordinate.",
+    unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
+    )
+    width: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Stroke width.",
     )
 
 
-DivPoint.update_forward_refs()
+DivStroke.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient.py` & `pydivkit-25.6.0/pydivkit/div/div_radial_gradient.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,56 +2,58 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_radial_gradient_center, div_radial_gradient_radius
 
 
 # Radial gradient.
 class DivRadialGradient(BaseDiv):
 
     def __init__(
         self, *,
-        colors: typing.List[str],
         type: str = "radial_gradient",
         center_x: typing.Optional[div_radial_gradient_center.DivRadialGradientCenter] = None,
         center_y: typing.Optional[div_radial_gradient_center.DivRadialGradientCenter] = None,
+        colors: typing.Optional[typing.Sequence[typing.Union[Expr, str]]] = None,
         radius: typing.Optional[div_radial_gradient_radius.DivRadialGradientRadius] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             center_x=center_x,
             center_y=center_y,
             colors=colors,
             radius=radius,
+            **kwargs,
         )
 
     type: str = Field(default="radial_gradient")
     center_x: typing.Optional[div_radial_gradient_center.DivRadialGradientCenter] = Field(
         description=(
             "Shift of the central point of the gradient relative to the "
             "left edge along the Xaxis."
         ),
     )
     center_y: typing.Optional[div_radial_gradient_center.DivRadialGradientCenter] = Field(
         description=(
             "Shift of the central point of the gradient relative to the "
-            "upper edge along the Yaxis."
+            "top edge along the Yaxis."
         ),
     )
-    colors: typing.List[str] = Field(
+    colors: typing.Sequence[typing.Union[Expr, str]] = Field(
         min_items=2, 
         description=(
-            "Colors. Gradient points will be located at an equal "
-            "distance from each other."
+            "Colors. Gradient points are located at an equal distance "
+            "from each other."
         ),
     )
     radius: typing.Optional[div_radial_gradient_radius.DivRadialGradientRadius] = Field(
         description="Radius of the gradient transition.",
     )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient_fixed_center.py` & `pydivkit-25.6.0/pydivkit/div/div_radial_gradient_fixed_center.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_size_unit
 
 
-# Fixed central point of the gradient.
+# Fixed coordinates of the central point of the gradient.
 class DivRadialGradientFixedCenter(BaseDiv):
 
     def __init__(
         self, *,
-        value: int,
         type: str = "fixed",
-        unit: typing.Optional[div_size_unit.DivSizeUnit] = None,
+        unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        value: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             unit=unit,
             value=value,
+            **kwargs,
         )
 
     type: str = Field(default="fixed")
-    unit: typing.Optional[div_size_unit.DivSizeUnit] = Field(
+    unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description=(
             "Unit of measurement. To learn more about units of size "
             "measurement, see [Layoutinside the "
             "card](../../layout.dita)."
         ),
     )
-    value: int = Field(
-        description="Shift value of the fixed central point of the gradient.",
+    value: typing.Union[Expr, int] = Field(
+        description="Coordinate value.",
     )
 
 
 DivRadialGradientFixedCenter.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_radial_gradient_relative_center.py` & `pydivkit-25.6.0/pydivkit/div/div_radial_gradient_relative_center.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,33 +2,32 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
-# Relative central point of the gradient.
+# Location of the central point of the gradient relative to the element borders.
 class DivRadialGradientRelativeCenter(BaseDiv):
 
     def __init__(
         self, *,
-        value: float,
         type: str = "relative",
+        value: typing.Optional[typing.Union[Expr, float]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             value=value,
+            **kwargs,
         )
 
     type: str = Field(default="relative")
-    value: float = Field(
-        description=(
-            "Shift value of the central relative point of the gradient "
-            "in the range `0..1`."
-        ),
+    value: typing.Union[Expr, float] = Field(
+        description="Coordinate value in the range \"0...1\".",
     )
 
 
 DivRadialGradientRelativeCenter.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_shadow.py` & `pydivkit-25.6.0/pydivkit/div/url_variable.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,45 +2,39 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_point
 
-
-# Element shadow.
-class DivShadow(BaseDiv):
+# Variable — URL as a string.
+class UrlVariable(BaseDiv):
 
     def __init__(
         self, *,
-        offset: div_point.DivPoint,
-        alpha: typing.Optional[float] = None,
-        blur: typing.Optional[int] = None,
-        color: typing.Optional[str] = None,
+        type: str = "url",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            alpha=alpha,
-            blur=blur,
-            color=color,
-            offset=offset,
+            type=type,
+            name=name,
+            value=value,
+            **kwargs,
         )
 
-    alpha: typing.Optional[float] = Field(
-        description="Shadow transparency.",
-    )
-    blur: typing.Optional[int] = Field(
-        description="Blur intensity.",
-    )
-    color: typing.Optional[str] = Field(
-        format="color", 
-        description="Shadow color.",
+    type: str = Field(default="url")
+    name: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description="Variable name.",
     )
-    offset: div_point.DivPoint = Field(
-        description="Shadow offset.",
+    value: typing.Union[Expr, str] = Field(
+        format="uri", 
+        description="Value.",
     )
 
 
-DivShadow.update_forward_refs()
+UrlVariable.update_forward_refs()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_slide_transition.py` & `pydivkit-25.6.0/pydivkit/div/div_slide_transition.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,63 +2,65 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_animation_interpolator, div_dimension
 
 
 # Slide animation.
 class DivSlideTransition(BaseDiv):
 
     def __init__(
         self, *,
         type: str = "slide",
         distance: typing.Optional[div_dimension.DivDimension] = None,
-        duration: typing.Optional[int] = None,
-        edge: typing.Optional[DivSlideTransitionEdge] = None,
-        interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = None,
-        start_delay: typing.Optional[int] = None,
+        duration: typing.Optional[typing.Union[Expr, int]] = None,
+        edge: typing.Optional[typing.Union[Expr, DivSlideTransitionEdge]] = None,
+        interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = None,
+        start_delay: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             distance=distance,
             duration=duration,
             edge=edge,
             interpolator=interpolator,
             start_delay=start_delay,
+            **kwargs,
         )
 
     type: str = Field(default="slide")
     distance: typing.Optional[div_dimension.DivDimension] = Field(
         description=(
             "A fixed value of an offset which the element starts "
             "appearing from or at which itfinishes disappearing. If no "
             "value is specified, the distance to the selectededge of a "
             "parent element is used."
         ),
     )
-    duration: typing.Optional[int] = Field(
+    duration: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Animation duration in milliseconds.",
     )
-    edge: typing.Optional[DivSlideTransitionEdge] = Field(
+    edge: typing.Optional[typing.Union[Expr, DivSlideTransitionEdge]] = Field(
         description=(
             "Edge of a parent element for one of the action types:where "
             "the element will movefrom when appearing;where the element "
             "will move to when disappearing."
         ),
     )
-    interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = Field(
+    interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = Field(
         description="Transition speed nature.",
     )
-    start_delay: typing.Optional[int] = Field(
+    start_delay: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Delay in milliseconds before animation starts.",
     )
 
 
 class DivSlideTransitionEdge(str, enum.Enum):
     LEFT = "left"
     TOP = "top"
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_slider.py` & `pydivkit-25.6.0/pydivkit/div/div_gif_image.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,250 +2,278 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
-    div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_drawable, div_edge_insets,
-    div_extension, div_focus, div_font_weight, div_point, div_size,
-    div_size_unit, div_tooltip, div_transform, div_transition_trigger,
-    div_visibility, div_visibility_action,
+    div_alignment_vertical, div_animation, div_appearance_transition,
+    div_aspect, div_background, div_border, div_change_transition,
+    div_disappear_action, div_edge_insets, div_extension, div_focus,
+    div_image_scale, div_size, div_tooltip, div_transform,
+    div_transition_trigger, div_visibility, div_visibility_action,
 )
 
 
-# Slider for selecting a value in the range.
-class DivSlider(BaseDiv):
+# Animated GIF image.
+class DivGifImage(BaseDiv):
 
     def __init__(
         self, *,
-        thumb_style: div_drawable.DivDrawable,
-        track_active_style: div_drawable.DivDrawable,
-        track_inactive_style: div_drawable.DivDrawable,
-        type: str = "slider",
+        type: str = "gif",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        action: typing.Optional[div_action.DivAction] = None,
+        action_animation: typing.Optional[div_animation.DivAnimation] = None,
+        actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        aspect: typing.Optional[div_aspect.DivAspect] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
+        gif_url: typing.Optional[typing.Union[Expr, str]] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        longtap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        max_value: typing.Optional[int] = None,
-        min_value: typing.Optional[int] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        row_span: typing.Optional[int] = None,
-        secondary_value_accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        thumb_secondary_style: typing.Optional[div_drawable.DivDrawable] = None,
-        thumb_secondary_text_style: typing.Optional[DivSliderTextStyle] = None,
-        thumb_secondary_value_variable: typing.Optional[str] = None,
-        thumb_text_style: typing.Optional[DivSliderTextStyle] = None,
-        thumb_value_variable: typing.Optional[str] = None,
-        tick_mark_active_style: typing.Optional[div_drawable.DivDrawable] = None,
-        tick_mark_inactive_style: typing.Optional[div_drawable.DivDrawable] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        placeholder_color: typing.Optional[typing.Union[Expr, str]] = None,
+        preload_required: typing.Optional[typing.Union[Expr, bool]] = None,
+        preview: typing.Optional[typing.Union[Expr, str]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        scale: typing.Optional[typing.Union[Expr, div_image_scale.DivImageScale]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
+            action=action,
+            action_animation=action_animation,
+            actions=actions,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
+            aspect=aspect,
             background=background,
             border=border,
             column_span=column_span,
+            content_alignment_horizontal=content_alignment_horizontal,
+            content_alignment_vertical=content_alignment_vertical,
+            disappear_actions=disappear_actions,
+            doubletap_actions=doubletap_actions,
             extensions=extensions,
             focus=focus,
+            gif_url=gif_url,
             height=height,
             id=id,
+            longtap_actions=longtap_actions,
             margins=margins,
-            max_value=max_value,
-            min_value=min_value,
             paddings=paddings,
+            placeholder_color=placeholder_color,
+            preload_required=preload_required,
+            preview=preview,
             row_span=row_span,
-            secondary_value_accessibility=secondary_value_accessibility,
+            scale=scale,
             selected_actions=selected_actions,
-            thumb_secondary_style=thumb_secondary_style,
-            thumb_secondary_text_style=thumb_secondary_text_style,
-            thumb_secondary_value_variable=thumb_secondary_value_variable,
-            thumb_style=thumb_style,
-            thumb_text_style=thumb_text_style,
-            thumb_value_variable=thumb_value_variable,
-            tick_mark_active_style=tick_mark_active_style,
-            tick_mark_inactive_style=tick_mark_inactive_style,
             tooltips=tooltips,
-            track_active_style=track_active_style,
-            track_inactive_style=track_inactive_style,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="slider")
+    type: str = Field(default="gif")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    action: typing.Optional[div_action.DivAction] = Field(
+        description=(
+            "One action when clicking on an element. Not used if the "
+            "`actions` parameter isset."
+        ),
+    )
+    action_animation: typing.Optional[div_animation.DivAnimation] = Field(
+        description=(
+            "Click animation. The web only supports the following "
+            "values: `fade`, `scale`,`native`, `no_animation` and `set`."
+        ),
+    )
+    actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Multiple actions when clicking on an element.",
+    )
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    aspect: typing.Optional[div_aspect.DivAspect] = Field(
+        description=(
+            "Fixed aspect ratio. The element\'s height is calculated "
+            "based on the width,ignoring the `height` value."
+        ),
+    )
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
+        description="Horizontal image alignment.",
+    )
+    content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
+        description="Vertical image alignment.",
+    )
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description="Action when double-clicking on an element.",
+    )
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
+    gif_url: typing.Union[Expr, str] = Field(
+        format="uri", 
+        description="Direct URL to a GIF image.",
+    )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
+    longtap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
+        min_items=1, 
+        description=(
+            "Action when long-clicking an element. Doesn\'t work on "
+            "devices that don\'t supporttouch gestures."
+        ),
+    )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
-    max_value: typing.Optional[int] = Field(
-        description="Maximum value. It must be greater than the minimum value.",
-    )
-    min_value: typing.Optional[int] = Field(
-        description="Minimum value.",
-    )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    row_span: typing.Optional[int] = Field(
+    placeholder_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Placeholder background before the image is loaded.",
+    )
+    preload_required: typing.Optional[typing.Union[Expr, bool]] = Field(
+        description="Background image must be loaded before the display.",
+    )
+    preview: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
+        description=(
+            "Image preview encoded in `base64`. It will be shown instead "
+            "of`placeholder_color` before the image is loaded. Format "
+            "`data url`:`data:[;base64],<data>`"
+        ),
+    )
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    secondary_value_accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for the secondary thumb.",
+    scale: typing.Optional[typing.Union[Expr, div_image_scale.DivImageScale]] = Field(
+        description=(
+            "Image scaling:`fit` places the entire image into the "
+            "element (free space isfilled with background);`fill` scales "
+            "the image to the element size and cuts offthe excess."
+        ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    thumb_secondary_style: typing.Optional[div_drawable.DivDrawable] = Field(
-        description="Style of the second pointer.",
-    )
-    thumb_secondary_text_style: typing.Optional[DivSliderTextStyle] = Field(
-        description="Text style in the second pointer.",
-    )
-    thumb_secondary_value_variable: typing.Optional[str] = Field(
-        min_length=1, 
-        description=(
-            "Name of the variable to store the current value of the "
-            "secondary thumb."
-        ),
-    )
-    thumb_style: div_drawable.DivDrawable = Field(
-        description="Style of the first pointer.",
-    )
-    thumb_text_style: typing.Optional[DivSliderTextStyle] = Field(
-        description="Text style in the first pointer.",
-    )
-    thumb_value_variable: typing.Optional[str] = Field(
-        min_length=1, 
-        description="Name of the variable to store the current thumb value.",
-    )
-    tick_mark_active_style: typing.Optional[div_drawable.DivDrawable] = Field(
-        description="Style of active serifs.",
-    )
-    tick_mark_inactive_style: typing.Optional[div_drawable.DivDrawable] = Field(
-        description="Style of inactive serifs.",
-    )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
-    track_active_style: div_drawable.DivDrawable = Field(
-        description="Style of the active part of a scale.",
-    )
-    track_inactive_style: div_drawable.DivDrawable = Field(
-        description="Style of the inactive part of a scale.",
-    )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -261,71 +289,33 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-class DivSliderTextStyle(BaseDiv):
-
-    def __init__(
-        self, *,
-        font_size: int,
-        font_size_unit: typing.Optional[div_size_unit.DivSizeUnit] = None,
-        font_weight: typing.Optional[div_font_weight.DivFontWeight] = None,
-        offset: typing.Optional[div_point.DivPoint] = None,
-        text_color: typing.Optional[str] = None,
-    ):
-        super().__init__(
-            font_size=font_size,
-            font_size_unit=font_size_unit,
-            font_weight=font_weight,
-            offset=offset,
-            text_color=text_color,
-        )
-
-    font_size: int = Field(
-        description="Font size.",
-    )
-    font_size_unit: typing.Optional[div_size_unit.DivSizeUnit] = Field(
-    )
-    font_weight: typing.Optional[div_font_weight.DivFontWeight] = Field(
-        description="Style.",
-    )
-    offset: typing.Optional[div_point.DivPoint] = Field(
-        description="Shift relative to the center.",
-    )
-    text_color: typing.Optional[str] = Field(
-        format="color", 
-        description="Text color.",
-    )
-
-
-DivSliderTextStyle.update_forward_refs()
-
-
-DivSlider.update_forward_refs()
+DivGifImage.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_state.py` & `pydivkit-25.6.0/pydivkit/div/div_indicator.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,143 +2,168 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
-    div, div_accessibility, div_action, div_alignment_horizontal,
-    div_alignment_vertical, div_animation, div_appearance_transition,
-    div_background, div_border, div_change_transition, div_edge_insets,
-    div_extension, div_focus, div_size, div_tooltip, div_transform,
-    div_transition_selector, div_transition_trigger, div_visibility,
+    div_accessibility, div_action, div_alignment_horizontal,
+    div_alignment_vertical, div_appearance_transition, div_background,
+    div_border, div_change_transition, div_disappear_action, div_edge_insets,
+    div_extension, div_fixed_size, div_focus, div_indicator_item_placement,
+    div_rounded_rectangle_shape, div_shape, div_size, div_tooltip,
+    div_transform, div_transition_trigger, div_visibility,
     div_visibility_action,
 )
 
 
-# It contains sets of states for visual elements and switches between them.
-class DivState(BaseDiv):
+# Progress indicator for [pager](div-pager.md).
+class DivIndicator(BaseDiv):
 
     def __init__(
         self, *,
-        states: typing.List[DivStateState],
-        type: str = "state",
+        type: str = "indicator",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        active_item_color: typing.Optional[typing.Union[Expr, str]] = None,
+        active_item_size: typing.Optional[typing.Union[Expr, float]] = None,
+        active_shape: typing.Optional[div_rounded_rectangle_shape.DivRoundedRectangleShape] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        animation: typing.Optional[typing.Union[Expr, DivIndicatorAnimation]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        default_state_id: typing.Optional[str] = None,
-        div_id: typing.Optional[str] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        inactive_item_color: typing.Optional[typing.Union[Expr, str]] = None,
+        inactive_minimum_shape: typing.Optional[div_rounded_rectangle_shape.DivRoundedRectangleShape] = None,
+        inactive_shape: typing.Optional[div_rounded_rectangle_shape.DivRoundedRectangleShape] = None,
+        items_placement: typing.Optional[div_indicator_item_placement.DivIndicatorItemPlacement] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
+        minimum_item_size: typing.Optional[typing.Union[Expr, float]] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        row_span: typing.Optional[int] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        pager_id: typing.Optional[typing.Union[Expr, str]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        shape: typing.Optional[div_shape.DivShape] = None,
+        space_between_centers: typing.Optional[div_fixed_size.DivFixedSize] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
-        transition_animation_selector: typing.Optional[div_transition_selector.DivTransitionSelector] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
+            active_item_color=active_item_color,
+            active_item_size=active_item_size,
+            active_shape=active_shape,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
+            animation=animation,
             background=background,
             border=border,
             column_span=column_span,
-            default_state_id=default_state_id,
-            div_id=div_id,
+            disappear_actions=disappear_actions,
             extensions=extensions,
             focus=focus,
             height=height,
             id=id,
+            inactive_item_color=inactive_item_color,
+            inactive_minimum_shape=inactive_minimum_shape,
+            inactive_shape=inactive_shape,
+            items_placement=items_placement,
             margins=margins,
+            minimum_item_size=minimum_item_size,
             paddings=paddings,
+            pager_id=pager_id,
             row_span=row_span,
             selected_actions=selected_actions,
-            states=states,
+            shape=shape,
+            space_between_centers=space_between_centers,
             tooltips=tooltips,
             transform=transform,
-            transition_animation_selector=transition_animation_selector,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
-    type: str = Field(default="state")
+    type: str = Field(default="indicator")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    active_item_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Active indicator color. @deprecated",
+    )
+    active_item_size: typing.Optional[typing.Union[Expr, float]] = Field(
+        description="A size multiplier for an active indicator. @deprecated",
+    )
+    active_shape: typing.Optional[div_rounded_rectangle_shape.DivRoundedRectangleShape] = Field(
+        description="Active indicator shape.",
+    )
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    animation: typing.Optional[typing.Union[Expr, DivIndicatorAnimation]] = Field(
+        description="Animation of switching between indicators.",
+    )
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    default_state_id: typing.Optional[str] = Field(
-        description=(
-            "ID of the status that will be set by default. If the "
-            "parameter isnt set, thefirst state of the `states` will be "
-            "set."
-        ),
-    )
-    div_id: typing.Optional[str] = Field(
-        description=(
-            "ID of an element to search in the hierarchy. The ID must be "
-            "unique at onehierarchy level. @deprecated"
-        ),
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
@@ -150,68 +175,88 @@
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
+    inactive_item_color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Indicator color. @deprecated",
+    )
+    inactive_minimum_shape: typing.Optional[div_rounded_rectangle_shape.DivRoundedRectangleShape] = Field(
+        description=(
+            "Inactive indicator shape, minimum size. Used when all the "
+            "indicators don\'t fit onthe screen."
+        ),
+    )
+    inactive_shape: typing.Optional[div_rounded_rectangle_shape.DivRoundedRectangleShape] = Field(
+        description="Indicator shape.",
+    )
+    items_placement: typing.Optional[div_indicator_item_placement.DivIndicatorItemPlacement] = Field(
+        description=(
+            "Indicator items placement mode:Default: Indicators\' width "
+            "is fixed and defined bythe `shape` parameters.Stretch: "
+            "Indicators are expanded to fill the entire width."
+        ),
+    )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
+    minimum_item_size: typing.Optional[typing.Union[Expr, float]] = Field(
+        description=(
+            "A size multiplier for a minimal indicator. It is used when "
+            "the required number ofindicators don\'t fit on the screen. "
+            "@deprecated"
+        ),
+    )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    row_span: typing.Optional[int] = Field(
+    pager_id: typing.Optional[typing.Union[Expr, str]] = Field(
+        description="ID of the pager that is a data source for an indicator.",
+    )
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    states: typing.List[DivStateState] = Field(
-        min_items=1, 
-        description=(
-            "States. Each element can have a few states with a different "
-            "layout. Transitionbetween states is performed using "
-            "[special scheme](../../interaction.dita) of "
-            "the[action](div-action.md) element."
-        ),
+    shape: typing.Optional[div_shape.DivShape] = Field(
+        description="Indicator shape. @deprecated",
+    )
+    space_between_centers: typing.Optional[div_fixed_size.DivFixedSize] = Field(
+        description="Spacing between indicator centers. @deprecated",
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
-        ),
-    )
-    transition_animation_selector: typing.Optional[div_transition_selector.DivTransitionSelector] = Field(
-        description=(
-            "It determines which events trigger transition animations. "
-            "@deprecated"
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -227,81 +272,39 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
-class DivStateState(BaseDiv):
-
-    def __init__(
-        self, *,
-        state_id: str,
-        animation_in: typing.Optional[div_animation.DivAnimation] = None,
-        animation_out: typing.Optional[div_animation.DivAnimation] = None,
-        div: typing.Optional[div.Div] = None,
-        swipe_out_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-    ):
-        super().__init__(
-            animation_in=animation_in,
-            animation_out=animation_out,
-            div=div,
-            state_id=state_id,
-            swipe_out_actions=swipe_out_actions,
-        )
-
-    animation_in: typing.Optional[div_animation.DivAnimation] = Field(
-        description=(
-            "State appearance animation. Use `transition_in` instead. "
-            "@deprecated"
-        ),
-    )
-    animation_out: typing.Optional[div_animation.DivAnimation] = Field(
-        description=(
-            "State disappearance animation. Use `transition_out` "
-            "instead. @deprecated"
-        ),
-    )
-    div: typing.Optional[div.Div] = Field(
-        description=(
-            "Contents. If the parameter is missing, the state won\'t be "
-            "displayed."
-        ),
-    )
-    state_id: str = Field(
-        description="State ID. It must be unique at one hierarchy level.",
-    )
-    swipe_out_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
-        min_items=1, 
-        description="Actions when swiping the state horizontally. @deprecated",
-    )
-
-
-DivStateState.update_forward_refs()
+class DivIndicatorAnimation(str, enum.Enum):
+    SCALE = "scale"
+    WORM = "worm"
+    SLIDER = "slider"
 
 
-DivState.update_forward_refs()
+DivIndicator.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_stroke.py` & `pydivkit-25.6.0/pydivkit/div/div_dimension.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,39 +2,35 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_size_unit
 
 
-# Stroke.
-class DivStroke(BaseDiv):
+# Element dimension value.
+class DivDimension(BaseDiv):
 
     def __init__(
         self, *,
-        color: str,
-        unit: typing.Optional[div_size_unit.DivSizeUnit] = None,
-        width: typing.Optional[int] = None,
+        unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        value: typing.Optional[typing.Union[Expr, float]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
-            color=color,
             unit=unit,
-            width=width,
+            value=value,
+            **kwargs,
         )
 
-    color: str = Field(
-        format="color", 
-        description="Stroke color.",
+    unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
     )
-    unit: typing.Optional[div_size_unit.DivSizeUnit] = Field(
-    )
-    width: typing.Optional[int] = Field(
-        description="Stroke width.",
+    value: typing.Union[Expr, float] = Field(
+        description="Value.",
     )
 
 
-DivStroke.update_forward_refs()
+DivDimension.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_tabs.py` & `pydivkit-25.6.0/pydivkit/div/div_tabs.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,78 +2,81 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
-    div_border, div_change_transition, div_corners_radius, div_edge_insets,
-    div_extension, div_focus, div_font_family, div_font_weight, div_size,
-    div_size_unit, div_tooltip, div_transform, div_transition_trigger,
+    div_border, div_change_transition, div_corners_radius, div_disappear_action,
+    div_edge_insets, div_extension, div_focus, div_font_family, div_font_weight,
+    div_size, div_size_unit, div_tooltip, div_transform, div_transition_trigger,
     div_visibility, div_visibility_action,
 )
 
 
 # Tabs. Height of the first tab is determined by its contents, and height of the
 # remaining [depends on the platform](../../location.dita#tabs).
 class DivTabs(BaseDiv):
 
     def __init__(
         self, *,
-        items: typing.List[DivTabsItem],
         type: str = "tabs",
         accessibility: typing.Optional[div_accessibility.DivAccessibility] = None,
-        alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = None,
-        alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = None,
-        alpha: typing.Optional[float] = None,
-        background: typing.Optional[typing.List[div_background.DivBackground]] = None,
+        alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
-        column_span: typing.Optional[int] = None,
-        dynamic_height: typing.Optional[bool] = None,
-        extensions: typing.Optional[typing.List[div_extension.DivExtension]] = None,
+        column_span: typing.Optional[typing.Union[Expr, int]] = None,
+        disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
+        dynamic_height: typing.Optional[typing.Union[Expr, bool]] = None,
+        extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
-        has_separator: typing.Optional[bool] = None,
+        has_separator: typing.Optional[typing.Union[Expr, bool]] = None,
         height: typing.Optional[div_size.DivSize] = None,
-        id: typing.Optional[str] = None,
+        id: typing.Optional[typing.Union[Expr, str]] = None,
+        items: typing.Optional[typing.Sequence[DivTabsItem]] = None,
         margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        restrict_parent_scroll: typing.Optional[bool] = None,
-        row_span: typing.Optional[int] = None,
-        selected_actions: typing.Optional[typing.List[div_action.DivAction]] = None,
-        selected_tab: typing.Optional[int] = None,
-        separator_color: typing.Optional[str] = None,
+        restrict_parent_scroll: typing.Optional[typing.Union[Expr, bool]] = None,
+        row_span: typing.Optional[typing.Union[Expr, int]] = None,
+        selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        selected_tab: typing.Optional[typing.Union[Expr, int]] = None,
+        separator_color: typing.Optional[typing.Union[Expr, str]] = None,
         separator_paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        switch_tabs_by_content_swipe_enabled: typing.Optional[bool] = None,
+        switch_tabs_by_content_swipe_enabled: typing.Optional[typing.Union[Expr, bool]] = None,
         tab_title_style: typing.Optional[DivTabsTabTitleStyle] = None,
         title_paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
-        tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = None,
+        tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
-        transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = None,
-        visibility: typing.Optional[div_visibility.DivVisibility] = None,
+        transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = None,
+        visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = None,
         visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = None,
-        visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = None,
+        visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = None,
         width: typing.Optional[div_size.DivSize] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             accessibility=accessibility,
             alignment_horizontal=alignment_horizontal,
             alignment_vertical=alignment_vertical,
             alpha=alpha,
             background=background,
             border=border,
             column_span=column_span,
+            disappear_actions=disappear_actions,
             dynamic_height=dynamic_height,
             extensions=extensions,
             focus=focus,
             has_separator=has_separator,
             height=height,
             id=id,
             items=items,
@@ -94,87 +97,92 @@
             transition_in=transition_in,
             transition_out=transition_out,
             transition_triggers=transition_triggers,
             visibility=visibility,
             visibility_action=visibility_action,
             visibility_actions=visibility_actions,
             width=width,
+            **kwargs,
         )
 
     type: str = Field(default="tabs")
     accessibility: typing.Optional[div_accessibility.DivAccessibility] = Field(
-        description="Accessibility for disabled people.",
+        description="Accessibility settings.",
     )
-    alignment_horizontal: typing.Optional[div_alignment_horizontal.DivAlignmentHorizontal] = Field(
+    alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
         description=(
             "Horizontal alignment of an element inside the parent "
             "element."
         ),
     )
-    alignment_vertical: typing.Optional[div_alignment_vertical.DivAlignmentVertical] = Field(
+    alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
         description=(
             "Vertical alignment of an element inside the parent element."
         ),
     )
-    alpha: typing.Optional[float] = Field(
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
         description=(
             "Sets transparency of the entire element: `0` — completely "
             "transparent, `1` —opaque."
         ),
     )
-    background: typing.Optional[typing.List[div_background.DivBackground]] = Field(
+    background: typing.Optional[typing.Sequence[div_background.DivBackground]] = Field(
         min_items=1, 
         description="Element background. It can contain multiple layers.",
     )
     border: typing.Optional[div_border.DivBorder] = Field(
         description="Element stroke.",
     )
-    column_span: typing.Optional[int] = Field(
+    column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    dynamic_height: typing.Optional[bool] = Field(
+    disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = Field(
+        min_items=1, 
+        description="Actions when an element disappears from the screen.",
+    )
+    dynamic_height: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "Updating height when changing the active element. In the "
             "browser, the value isalways `true`."
         ),
     )
-    extensions: typing.Optional[typing.List[div_extension.DivExtension]] = Field(
+    extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = Field(
         min_items=1, 
         description=(
             "Extensions for additional processing of an element. The "
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
-    has_separator: typing.Optional[bool] = Field(
+    has_separator: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="A separating line between tabs and contents.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
             "Element height. For Android: if there is text in this or in "
             "a child element,specify height in `sp` to scale the element "
             "together with the text. To learn moreabout units of size "
             "measurement, see [Layout inside the "
             "card](../../layout.dita)."
         ),
     )
-    id: typing.Optional[str] = Field(
+    id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
             "Element ID. It must be unique within the root element. It "
             "is used as`accessibilityIdentifier` on iOS."
         ),
     )
-    items: typing.List[DivTabsItem] = Field(
+    items: typing.Sequence[DivTabsItem] = Field(
         min_items=1, 
         description=(
             "Tabs. Transition between tabs can be "
             "implementedusing:`div-action://set_current_item?id=&item=` "
             "— set the current tab with anordinal number `item` inside "
             "an element, with the "
             "specified`id`;`div-action://set_next_item?id=[&overflow={cl"
@@ -191,68 +199,67 @@
     )
     margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="External margins from the element stroke.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
-    restrict_parent_scroll: typing.Optional[bool] = Field(
+    restrict_parent_scroll: typing.Optional[typing.Union[Expr, bool]] = Field(
         description=(
             "If the parameter is enabled, tabs won\'t transmit the "
             "scroll gesture to the parentelement."
         ),
     )
-    row_span: typing.Optional[int] = Field(
+    row_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a string of the [grid](div-grid.md) "
             "element."
         ),
     )
-    selected_actions: typing.Optional[typing.List[div_action.DivAction]] = Field(
+    selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
-    selected_tab: typing.Optional[int] = Field(
+    selected_tab: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Ordinal number of the tab that will be opened by default.",
     )
-    separator_color: typing.Optional[str] = Field(
+    separator_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Separator color.",
     )
     separator_paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description=(
             "Indents from the separating line. Not used if "
             "`has_separator = false`."
         ),
     )
-    switch_tabs_by_content_swipe_enabled: typing.Optional[bool] = Field(
+    switch_tabs_by_content_swipe_enabled: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="Switching tabs by scrolling through the contents.",
     )
     tab_title_style: typing.Optional[DivTabsTabTitleStyle] = Field(
         description="Design style of tab titles.",
     )
     title_paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Indents in the tab name.",
     )
-    tooltips: typing.Optional[typing.List[div_tooltip.DivTooltip]] = Field(
+    tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = Field(
         min_items=1, 
         description=(
             "Tooltips linked to an element. A tooltip can be shown "
             "by`div-action://show_tooltip?id=`, hidden by "
             "`div-action://hide_tooltip?id=` where`id` — tooltip id."
         ),
     )
     transform: typing.Optional[div_transform.DivTransform] = Field(
         description=(
-            "Transformation of the element. Applies the passed transform "
-            "to the element. Thecontent that does not fit into the "
-            "original view will be cut off."
+            "Applies the passed transformation to the element. Content "
+            "that doesn\'t fit intothe original view area is cut off."
         ),
     )
     transition_change: typing.Optional[div_change_transition.DivChangeTransition] = Field(
         description=(
             "Change animation. It is played when the position or size of "
             "an element changes inthe new layout."
         ),
@@ -268,58 +275,60 @@
     )
     transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = Field(
         description=(
             "Disappearance animation. It is played when an element "
             "disappears in the newlayout."
         ),
     )
-    transition_triggers: typing.Optional[typing.List[div_transition_trigger.DivTransitionTrigger]] = Field(
+    transition_triggers: typing.Optional[typing.Sequence[typing.Union[Expr, div_transition_trigger.DivTransitionTrigger]]] = Field(
         min_items=1, 
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
-    visibility: typing.Optional[div_visibility.DivVisibility] = Field(
+    visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
             "`visibility_actions`parameter is set."
         ),
     )
-    visibility_actions: typing.Optional[typing.List[div_visibility_action.DivVisibilityAction]] = Field(
+    visibility_actions: typing.Optional[typing.Sequence[div_visibility_action.DivVisibilityAction]] = Field(
         min_items=1, 
         description="Actions when an element appears on the screen.",
     )
     width: typing.Optional[div_size.DivSize] = Field(
         description="Element width.",
     )
 
 
 # Tab.
 class DivTabsItem(BaseDiv):
 
     def __init__(
         self, *,
-        div: div.Div,
-        title: str,
+        div: typing.Optional[div.Div] = None,
+        title: typing.Optional[typing.Union[Expr, str]] = None,
         title_click_action: typing.Optional[div_action.DivAction] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             div=div,
             title=title,
             title_click_action=title_click_action,
+            **kwargs,
         )
 
     div: div.Div = Field(
         description="Tab contents.",
     )
-    title: str = Field(
+    title: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Tab title.",
     )
     title_click_action: typing.Optional[div_action.DivAction] = Field(
         description="Action when clicking on the active tab title.",
     )
 
@@ -328,32 +337,33 @@
 
 
 # Design style of tab titles.
 class DivTabsTabTitleStyle(BaseDiv):
 
     def __init__(
         self, *,
-        active_background_color: typing.Optional[str] = None,
-        active_font_weight: typing.Optional[div_font_weight.DivFontWeight] = None,
-        active_text_color: typing.Optional[str] = None,
-        animation_duration: typing.Optional[int] = None,
-        animation_type: typing.Optional[TabTitleStyleAnimationType] = None,
-        corner_radius: typing.Optional[int] = None,
+        active_background_color: typing.Optional[typing.Union[Expr, str]] = None,
+        active_font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
+        active_text_color: typing.Optional[typing.Union[Expr, str]] = None,
+        animation_duration: typing.Optional[typing.Union[Expr, int]] = None,
+        animation_type: typing.Optional[typing.Union[Expr, TabTitleStyleAnimationType]] = None,
+        corner_radius: typing.Optional[typing.Union[Expr, int]] = None,
         corners_radius: typing.Optional[div_corners_radius.DivCornersRadius] = None,
-        font_family: typing.Optional[div_font_family.DivFontFamily] = None,
-        font_size: typing.Optional[int] = None,
-        font_size_unit: typing.Optional[div_size_unit.DivSizeUnit] = None,
-        font_weight: typing.Optional[div_font_weight.DivFontWeight] = None,
-        inactive_background_color: typing.Optional[str] = None,
-        inactive_font_weight: typing.Optional[div_font_weight.DivFontWeight] = None,
-        inactive_text_color: typing.Optional[str] = None,
-        item_spacing: typing.Optional[int] = None,
-        letter_spacing: typing.Optional[float] = None,
-        line_height: typing.Optional[int] = None,
+        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_size: typing.Optional[typing.Union[Expr, int]] = None,
+        font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
+        inactive_background_color: typing.Optional[typing.Union[Expr, str]] = None,
+        inactive_font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
+        inactive_text_color: typing.Optional[typing.Union[Expr, str]] = None,
+        item_spacing: typing.Optional[typing.Union[Expr, int]] = None,
+        letter_spacing: typing.Optional[typing.Union[Expr, float]] = None,
+        line_height: typing.Optional[typing.Union[Expr, int]] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             active_background_color=active_background_color,
             active_font_weight=active_font_weight,
             active_text_color=active_text_color,
             animation_duration=animation_duration,
             animation_type=animation_type,
@@ -366,86 +376,84 @@
             inactive_background_color=inactive_background_color,
             inactive_font_weight=inactive_font_weight,
             inactive_text_color=inactive_text_color,
             item_spacing=item_spacing,
             letter_spacing=letter_spacing,
             line_height=line_height,
             paddings=paddings,
+            **kwargs,
         )
 
-    active_background_color: typing.Optional[str] = Field(
+    active_background_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Background color of the active tab title.",
     )
-    active_font_weight: typing.Optional[div_font_weight.DivFontWeight] = Field(
+    active_font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = Field(
         description="Active tab title style.",
     )
-    active_text_color: typing.Optional[str] = Field(
+    active_text_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Color of the active tab title text.",
     )
-    animation_duration: typing.Optional[int] = Field(
+    animation_duration: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Duration of active title change animation.",
     )
-    animation_type: typing.Optional[TabTitleStyleAnimationType] = Field(
+    animation_type: typing.Optional[typing.Union[Expr, TabTitleStyleAnimationType]] = Field(
         description="Active title change animation.",
     )
-    corner_radius: typing.Optional[int] = Field(
+    corner_radius: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Title corner rounding radius. If the parameter isn\'t "
             "specified, the rounding ismaximum (half of the smallest "
             "size). Not used if the `corners_radius` parameteris set."
         ),
     )
     corners_radius: typing.Optional[div_corners_radius.DivCornersRadius] = Field(
         description=(
             "Rounding radii of corners of multiple titles. Empty values "
             "are replaced by`corner_radius`."
         ),
     )
-    font_family: typing.Optional[div_font_family.DivFontFamily] = Field(
+    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
         description=(
             "Font family:`text` — a standard text font;`display` — a "
             "family of fonts with alarge font size."
         ),
     )
-    font_size: typing.Optional[int] = Field(
+    font_size: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Title font size.",
     )
-    font_size_unit: typing.Optional[div_size_unit.DivSizeUnit] = Field(
+    font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description="Units of title font size measurement.",
     )
-    font_weight: typing.Optional[div_font_weight.DivFontWeight] = Field(
+    font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = Field(
         description=(
             "Style. Use `active_font_weight` and `inactive_font_weight` "
             "instead. @deprecated"
         ),
     )
-    inactive_background_color: typing.Optional[str] = Field(
+    inactive_background_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Background color of the inactive tab title.",
     )
-    inactive_font_weight: typing.Optional[div_font_weight.DivFontWeight] = Field(
+    inactive_font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = Field(
         description="Inactive tab title style.",
     )
-    inactive_text_color: typing.Optional[str] = Field(
+    inactive_text_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Color of the inactive tab title text.",
     )
-    item_spacing: typing.Optional[int] = Field(
+    item_spacing: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Spacing between neighbouring tab titles.",
     )
-    letter_spacing: typing.Optional[float] = Field(
+    letter_spacing: typing.Optional[typing.Union[Expr, float]] = Field(
         description="Spacing between title characters.",
     )
-    line_height: typing.Optional[int] = Field(
-        description=(
-            "Line spacing of the text range. The count is taken from the "
-            "font baseline."
-        ),
+    line_height: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Line spacing of the text.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Indents around the tab title.",
     )
 
 
 class TabTitleStyleAnimationType(str, enum.Enum):
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_transition_base.py` & `pydivkit-25.6.0/pydivkit/div/div_transition_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_animation_interpolator
 
 
 class DivTransitionBase(BaseDiv):
 
     def __init__(
         self, *,
-        duration: typing.Optional[int] = None,
-        interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = None,
-        start_delay: typing.Optional[int] = None,
+        duration: typing.Optional[typing.Union[Expr, int]] = None,
+        interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = None,
+        start_delay: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             duration=duration,
             interpolator=interpolator,
             start_delay=start_delay,
+            **kwargs,
         )
 
-    duration: typing.Optional[int] = Field(
+    duration: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Animation duration in milliseconds.",
     )
-    interpolator: typing.Optional[div_animation_interpolator.DivAnimationInterpolator] = Field(
+    interpolator: typing.Optional[typing.Union[Expr, div_animation_interpolator.DivAnimationInterpolator]] = Field(
         description="Transition speed nature.",
     )
-    start_delay: typing.Optional[int] = Field(
+    start_delay: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Delay in milliseconds before animation starts.",
     )
 
 
 DivTransitionBase.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_variable.py` & `pydivkit-25.6.0/pydivkit/div/div_variable.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import enum
 import typing
 from typing import Union
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     boolean_variable, color_variable, integer_variable, number_variable,
     string_variable, url_variable,
 )
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/div_visibility_action.py` & `pydivkit-25.6.0/pydivkit/div/div_disappear_action.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,83 +2,85 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_download_callbacks
 
 
-# Actions performed when an element becomes visible.
-class DivVisibilityAction(BaseDiv):
+# Actions performed when an element becomes invisible.
+class DivDisappearAction(BaseDiv):
 
     def __init__(
         self, *,
-        log_id: str,
+        disappear_duration: typing.Optional[typing.Union[Expr, int]] = None,
         download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = None,
-        log_limit: typing.Optional[int] = None,
+        log_id: typing.Optional[typing.Union[Expr, str]] = None,
+        log_limit: typing.Optional[typing.Union[Expr, int]] = None,
         payload: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        referer: typing.Optional[str] = None,
-        url: typing.Optional[str] = None,
-        visibility_duration: typing.Optional[int] = None,
-        visibility_percentage: typing.Optional[int] = None,
+        referer: typing.Optional[typing.Union[Expr, str]] = None,
+        url: typing.Optional[typing.Union[Expr, str]] = None,
+        visibility_percentage: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
+            disappear_duration=disappear_duration,
             download_callbacks=download_callbacks,
             log_id=log_id,
             log_limit=log_limit,
             payload=payload,
             referer=referer,
             url=url,
-            visibility_duration=visibility_duration,
             visibility_percentage=visibility_percentage,
+            **kwargs,
         )
 
+    disappear_duration: typing.Optional[typing.Union[Expr, int]] = Field(
+        description=(
+            "Time in milliseconds during which an element must be "
+            "invisible to trigger`disappear-action`."
+        ),
+    )
     download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = Field(
         description=(
             "Callbacks that are called after "
             "[dataloading](../../interaction.dita#loading-data)."
         ),
     )
-    log_id: str = Field(
+    log_id: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Logging ID.",
     )
-    log_limit: typing.Optional[int] = Field(
+    log_limit: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Limit on the number of loggings. If `0`, the limit is "
             "removed."
         ),
     )
     payload: typing.Optional[typing.Dict[str, typing.Any]] = Field(
         description="Additional parameters, passed to the host application.",
     )
-    referer: typing.Optional[str] = Field(
+    referer: typing.Optional[typing.Union[Expr, str]] = Field(
         format="uri", 
         description="Referer URL for logging.",
     )
-    url: typing.Optional[str] = Field(
+    url: typing.Optional[typing.Union[Expr, str]] = Field(
         format="uri", 
         description=(
             "URL. Possible values: `url` or `div-action://`. To learn "
             "more, see [Interactionwith "
             "elements](../../interaction.dita)."
         ),
     )
-    visibility_duration: typing.Optional[int] = Field(
-        description=(
-            "Time in milliseconds during which an element must be "
-            "visible to trigger`visibility-action`."
-        ),
-    )
-    visibility_percentage: typing.Optional[int] = Field(
+    visibility_percentage: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Percentage of the visible part of an element that triggers "
-            "`visibility-action`."
+            "`disappear-action`."
         ),
     )
 
 
-DivVisibilityAction.update_forward_refs()
+DivDisappearAction.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/integer_variable.py` & `pydivkit-25.6.0/pydivkit/div/integer_variable.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
 # An integer variable.
 class IntegerVariable(BaseDiv):
 
     def __init__(
         self, *,
-        name: str,
-        value: int,
         type: str = "integer",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Union[Expr, int]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             name=name,
             value=value,
+            **kwargs,
         )
 
     type: str = Field(default="integer")
-    name: str = Field(
+    name: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Variable name.",
     )
-    value: int = Field(
+    value: typing.Union[Expr, int] = Field(
         description="Value.",
     )
 
 
 IntegerVariable.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/number_variable.py` & `pydivkit-25.6.0/pydivkit/div/div_change_set_transition.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
+from . import div_change_transition
 
-# A floating-point variable.
-class NumberVariable(BaseDiv):
+
+# Animations.
+class DivChangeSetTransition(BaseDiv):
 
     def __init__(
         self, *,
-        name: str,
-        value: float,
-        type: str = "number",
+        type: str = "set",
+        items: typing.Optional[typing.Sequence[div_change_transition.DivChangeTransition]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            name=name,
-            value=value,
+            items=items,
+            **kwargs,
         )
 
-    type: str = Field(default="number")
-    name: str = Field(
-        min_length=1, 
-        description="Variable name.",
-    )
-    value: float = Field(
-        description="Value.",
+    type: str = Field(default="set")
+    items: typing.Sequence[div_change_transition.DivChangeTransition] = Field(
+        min_items=1, 
+        description="List of animations.",
     )
 
 
-NumberVariable.update_forward_refs()
+DivChangeSetTransition.update_forward_refs()
```

### Comparing `pydivkit-13.0.0b0/pydivkit/div/string_variable.py` & `pydivkit-25.6.0/pydivkit/div/color_variable.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 # flake8: noqa: F401, F405, F811
 
 from __future__ import annotations
 
 import enum
 import typing
 
-from pydivkit.core import BaseDiv, Field
+from pydivkit.core import BaseDiv, Expr, Field
 
 
-# A string variable.
-class StringVariable(BaseDiv):
+# Variable — HEX color as a string.
+class ColorVariable(BaseDiv):
 
     def __init__(
         self, *,
-        name: str,
-        value: str,
-        type: str = "string",
+        type: str = "color",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Union[Expr, str]] = None,
+        **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             name=name,
             value=value,
+            **kwargs,
         )
 
-    type: str = Field(default="string")
-    name: str = Field(
+    type: str = Field(default="color")
+    name: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Variable name.",
     )
-    value: str = Field(
+    value: typing.Union[Expr, str] = Field(
+        format="color", 
         description="Value.",
     )
 
 
-StringVariable.update_forward_refs()
+ColorVariable.update_forward_refs()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydivkit-13.0.0b0/pyproject.toml` & `pydivkit-25.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "pydivkit"
-version = "13.0.0b0"
+version = "25.6.0"
 description = "DivKit python library"
 readme = "README.md"
 repository = "https://github.com/divkit/divkit/tree/main/json-builder/python"
 keywords = ["divkit", "sdk"]
 authors = [
     "Vladislav Bakaev <bakaev-vlad@yandex-team.ru>",
-    "Dmitry Orlov <mosquito@yandex-team.ru>"
+    "Pavel Mosein <p-mosein@yandex-team.ru>",
+    "Dmitry Orlov <mosquito@yandex-team.ru>",
 ]
 include = ["pydivkit/div/*", "pydivkit/py.typed"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Information Technology",
@@ -28,25 +29,21 @@
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-[tool.poetry.dev-dependencies]
-autoflake = "^1.7.7"
+[tool.poetry.group.dev.dependencies]
 gray = "^0.10.2"
 mypy = "^0.931"
-pre-commit = "^2.17.0"
-pylama = "^8.3.0"
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.0.1"
 pytest-asyncio = "^0.18.1"
-teamcity-messages = "^1.31"
-yesqa = "^1.3.0"
-isort = "^5.10.1"
 
 [tool.mypy]
 cache_dir = "/dev/null"
 strict = true
 ignore_missing_imports = true
 allow_subclassing_any = true
 allow_untyped_calls = true
```

### Comparing `pydivkit-13.0.0b0/setup.py` & `pydivkit-25.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,440 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydivkit
+Version: 25.6.0
+Summary: DivKit python library
+Home-page: https://github.com/divkit/divkit/tree/main/json-builder/python
+Keywords: divkit,sdk
+Author: Vladislav Bakaev
+Author-email: bakaev-vlad@yandex-team.ru
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Russian
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Typing :: Typed
+Project-URL: Repository, https://github.com/divkit/divkit/tree/main/json-builder/python
+Description-Content-Type: text/markdown
 
-packages = \
-['pydivkit', 'pydivkit.core', 'pydivkit.core.types', 'pydivkit.div']
+PyDIVKit examples
+=================
 
-package_data = \
-{'': ['*']}
+This library is designed to work with [DivKit](http://divkit.tech/) with python.
 
-setup_kwargs = {
-    'name': 'pydivkit',
-    'version': '13.0.0b0',
-    'description': 'DivKit python library',
-    'long_description': 'PyDIVKit examples\n=================\n\nThis library is for working with DivKit with python.\n\nFeatures:\n* Declarative and imperative DivKit blocks definition\n* Native Type-hints support\n* Complete object-oriented API\n* IDE type checks and suggestions\n\nObject construction\n-------------------\n\nThe main idea is a provides ability to construct blocks by python objects.\n\n```python\nimport json\nimport pydivkit as dk\n\ncontainer = dk.DivContainer(\n    items=[\n        dk.DivGallery(\n            items=[\n                dk.DivText(text="Hello from pydivkit")\n            ]\n        )\n    ]\n)\n\nprint(json.dumps(container.dict(), indent=1))\n# {\n#  "type": "container",\n#  "items": [\n#   {\n#    "type": "gallery",\n#    "items": [\n#     {\n#      "type": "text",\n#      "text": "Hello from pydivkit"\n#     }\n#    ]\n#   }\n#  ]\n# }\n```\n\nSlider example\n--------------\n\nFollowing code is a rewritten slider example using pydivkit.\n\n```python\nimport pydivkit as dk\n\n\nslider = dk.DivData(\n    log_id="sample_card",\n    states=[\n        dk.DivDataState(\n            state_id=0,\n            div=dk.DivSlider(\n                width=dk.DivMatchParentSize(),\n                max_value=10,\n                min_value=1,\n                thumb_style=dk.DivShapeDrawable(\n                    color="#00b300",\n                    stroke=dk.DivStroke(\n                        color="#ffffff",\n                        width=3,\n                    ),\n                    shape=dk.DivRoundedRectangleShape(\n                        item_width=dk.DivFixedSize(value=32),\n                        item_height=dk.DivFixedSize(value=32),\n                        corner_radius=dk.DivFixedSize(value=100)\n                    ),\n                ),\n                track_active_style=dk.DivShapeDrawable(\n                    color="#00b300",\n                    shape=dk.DivRoundedRectangleShape(\n                        item_height=dk.DivFixedSize(value=6)\n                    )\n                ),\n                track_inactive_style=dk.DivShapeDrawable(\n                    color="#20000000",\n                    shape=dk.DivRoundedRectangleShape(\n                        item_height=dk.DivFixedSize(value=6)\n                    )\n                )\n            )\n        )\n    ]\n)\n\n```\n\nThis example might be serialised like this:\n\n```python\nimport json\n\nprint(json.dumps(slider.dict(), indent=1))\n# {\n#  "log_id": "sample_card",\n#  "states": [\n#   {\n#    "div": {\n#     "type": "slider",\n#     "max_value": 10,\n#     "min_value": 1,\n#     "thumb_style": {\n#      "type": "shape_drawable",\n#      "color": "#00b300",\n#      "shape": {\n#       "type": "rounded_rectangle",\n#       "corner_radius": {\n#        "type": "fixed",\n#        "value": 100\n#       },\n#       "item_height": {\n#        "type": "fixed",\n#        "value": 32\n#       },\n#       "item_width": {\n#        "type": "fixed",\n#        "value": 32\n#       }\n#      },\n#      "stroke": {\n#       "color": "#ffffff",\n#       "width": 3\n#      }\n#     },\n#     "track_active_style": {\n#      "type": "shape_drawable",\n#      "color": "#00b300",\n#      "shape": {\n#       "type": "rounded_rectangle",\n#       "item_height": {\n#        "type": "fixed",\n#        "value": 6\n#       }\n#      }\n#     },\n#     "track_inactive_style": {\n#      "type": "shape_drawable",\n#      "color": "#20000000",\n#      "shape": {\n#       "type": "rounded_rectangle",\n#       "item_height": {\n#        "type": "fixed",\n#        "value": 6\n#       }\n#      }\n#     },\n#     "width": {\n#      "type": "match_parent"\n#     }\n#    },\n#    "state_id": 0\n#   }\n#  ]\n# }\n```\n\nTemplating and DRY\n------------------\n\nOf course building blocks from your code every time manually it\'s\na very boring. So the first idea it\'s a move initialization of the \nDivKit objects to the functions.\n\n```python\n# Naive DRY example which strictly non-recommended\nimport pydivkit as dk\n\n\ndef get_size(value: int = 32) -> dk.DivFixedSize:\n    return dk.DivFixedSize(value=value)\n\n\ndef get_shape() -> dk.DivShape:\n    return dk.DivShape(\n        item_width=get_size(),\n        item_height=get_size(),\n        corner_radius=get_size(100)\n    )\n\n    \nslider_shape = get_shape()\n\nslider = dk.DivData(\n    log_id="sample_card",\n    states=[\n        dk.DivDataState(\n            # other arguments\n            div=dk.DivSlider(\n                thumb_style=dk.DivShapeDrawable(\n                    shape=slider_shape,\n                    # other arguments\n                ),\n                # other arguments\n            )\n        )\n    ]\n)\n```\n\nLooks a little better, but this approach doesn\'t scale well. To simplify layout \nand save traffic, DivKit has templates. This is a way to layout similar elements\nwithout having to declare the complete json, but just declare a template and use\nthis many times in similar items.\n\n**PyDivKit supports defining templates through the inheritance.**\n\nLet\'s define an example card.\n\n```python\nimport json\n\nimport pydivkit as dk\n\n\nclass CategoriesItem(dk.DivContainer):\n    """\n    Class inherited from dk.DivContainer will have a template\n    """\n\n    # Special object for mark this fields a DivKit field in template\n    icon_url: str = dk.Field()\n    text: str = dk.Field()\n\n    # Set defaults layout for in the template\n    width = dk.DivWrapContentSize()\n    background = [dk.DivSolidBackground(color="#f0f0f0")]\n    content_alignment_vertical = dk.DivAlignmentVertical.CENTER\n    orientation = dk.DivContainerOrientation.HORIZONTAL\n    paddings = dk.DivEdgeInsets(left=12, right=12, top=10, bottom=10)\n    border = dk.DivBorder(corner_radius=12)\n    items = [\n        dk.DivImage(\n            width=dk.DivFixedSize(value=20),\n            height=dk.DivFixedSize(value=20),\n            margins=dk.DivEdgeInsets(right=6),\n\n            # Special object Ref it\'s a reference for Field property\n            image_url=dk.Ref(icon_url),\n        ),\n        dk.DivText(\n            width=dk.DivWrapContentSize(),\n            max_lines=1,\n\n            # Special object Ref it\'s a reference for Field property\n            text=dk.Ref(text),\n        ),\n    ]\n\n\nBASE_URL = "https://leonardo.edadeal.io/dyn/re/segments/level1/96"\n\n\n# So after class definition you might use all the `Field` marked property\n# names as an argument.\n\ngallery = dk.DivGallery(\n    items=[\n        CategoriesItem(\n            text="Food", icon_url=f"{BASE_URL}/food.png",\n        ),\n        CategoriesItem(\n            text="Alcohol", icon_url=f"{BASE_URL}/alcohol.png",\n        ),\n        CategoriesItem(\n            text="Household", icon_url=f"{BASE_URL}/household.png",\n        ),\n    ]\n)\n\nprint(json.dumps(dk.make_div(gallery), indent=1, ensure_ascii=False))\n# {\n#  "templates": {\n#   "__main__.CategoriesItem": {\n#    "type": "container",\n#    "background": [\n#     {\n#      "type": "solid",\n#      "color": "#f0f0f0"\n#     }\n#    ],\n#    "border": {\n#     "corner_radius": 12\n#    },\n#    "content_alignment_vertical": "center",\n#    "items": [\n#     {\n#      "type": "image",\n#      "height": {\n#       "type": "fixed",\n#       "value": 20\n#      },\n#      "$image_url": "icon_url",\n#      "margins": {\n#       "right": 6\n#      },\n#      "width": {\n#       "type": "fixed",\n#       "value": 20\n#      }\n#     },\n#     {\n#      "type": "text",\n#      "max_lines": 1,\n#      "$text": "text",\n#      "width": {\n#       "type": "wrap_content"\n#      }\n#     }\n#    ],\n#    "orientation": "horizontal",\n#    "paddings": {\n#     "bottom": 10,\n#     "left": 12,\n#     "right": 12,\n#     "top": 10\n#    },\n#    "width": {\n#     "type": "wrap_content"\n#    }\n#   }\n#  },\n#  "card": {\n#   "log_id": "card",\n#   "states": [\n#    {\n#     "div": {\n#      "type": "gallery",\n#      "items": [\n#       {\n#        "type": "__main__.CategoriesItem",\n#        "icon_url": "https://leonardo.edadeal.io/dyn/re/segments/level1/96/food.png",\n#        "text": "Food"\n#       },\n#       {\n#        "type": "__main__.CategoriesItem",\n#        "icon_url": "https://leonardo.edadeal.io/dyn/re/segments/level1/96/alcohol.png",\n#        "text": "Alcohol"\n#       },\n#       {\n#        "type": "__main__.CategoriesItem",\n#        "icon_url": "https://leonardo.edadeal.io/dyn/re/segments/level1/96/household.png",\n#        "text": "Household"\n#       }\n#      ]\n#     },\n#     "state_id": 0\n#    }\n#   ]\n#  }\n# }\n```\n\nTemplate names\n--------------\n\nBy default, templates are collecting by the metaclass into shared storage when \nthe class is declaring at import time, and have the \nformat `{module_name}.{class_name}`.\n\nThe following example, which I am sure will not occur in the wild, shows a \nwarning if suddenly the names of the classes, and hence the templates, conflict.\n\n```python\nimport pydivkit as dk\n\n\nclass MyTemplate(dk.DivContainer):\n    width = dk.DivWrapContentSize()\n\n\nclass MyTemplate(dk.DivContainer):\n    pass\n\n# RuntimeWarning: Template \'test.MyTemplate\' already defined in \n# <class \'test.MyTemplate\'> and will be replaced to <class \'test.MyTemplate\'>\n```\n\nAlso, if you do not want to show the structure of your project to the outside, \nor for some reason you need to make the example above clean, you can rename the\ntemplate by declaring a special attribute `__template_name__`\n\n```python\nimport pydivkit as dk\n\n\nclass MyTemplate(dk.DivContainer):\n    width = dk.DivWrapContentSize()\n\nprint(MyTemplate.template_name)\n# >>> test.MyTemplate\n\nclass MyTemplate(dk.DivContainer):\n    __template_name__ = "MyTemplate2"\n\nprint(MyTemplate.template_name)\n# >>> MyTemplate2\n```\n',
-    'author': 'Vladislav Bakaev',
-    'author_email': 'bakaev-vlad@yandex-team.ru',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/divkit/divkit/tree/main/json-builder/python',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+Features:
+* Declarative and imperative DivKit blocks definition
+* Native Type-hints support
+* Complete object-oriented API
+* IDE type checks and suggestions
 
+Object construction
+-------------------
+
+The main idea is to provide a tool for creating blocks using Python objects.
+
+```python
+import json
+import pydivkit as dk
+
+container = dk.DivContainer(
+    items=[
+        dk.DivGallery(
+            items=[
+                dk.DivText(text="Hello from pydivkit")
+            ]
+        )
+    ]
+)
+
+print(json.dumps(container.dict(), indent=1))
+# {
+#  "type": "container",
+#  "items": [
+#   {
+#    "type": "gallery",
+#    "items": [
+#     {
+#      "type": "text",
+#      "text": "Hello from pydivkit"
+#     }
+#    ]
+#   }
+#  ]
+# }
+```
+
+Slider example
+--------------
+
+Following code is a rewritten slider example using pydivkit.
+
+```python
+import pydivkit as dk
+
+
+slider = dk.DivData(
+    log_id="sample_card",
+    states=[
+        dk.DivDataState(
+            state_id=0,
+            div=dk.DivSlider(
+                width=dk.DivMatchParentSize(),
+                max_value=10,
+                min_value=1,
+                thumb_style=dk.DivShapeDrawable(
+                    color="#00b300",
+                    stroke=dk.DivStroke(
+                        color="#ffffff",
+                        width=3,
+                    ),
+                    shape=dk.DivRoundedRectangleShape(
+                        item_width=dk.DivFixedSize(value=32),
+                        item_height=dk.DivFixedSize(value=32),
+                        corner_radius=dk.DivFixedSize(value=100)
+                    ),
+                ),
+                track_active_style=dk.DivShapeDrawable(
+                    color="#00b300",
+                    shape=dk.DivRoundedRectangleShape(
+                        item_height=dk.DivFixedSize(value=6)
+                    )
+                ),
+                track_inactive_style=dk.DivShapeDrawable(
+                    color="#20000000",
+                    shape=dk.DivRoundedRectangleShape(
+                        item_height=dk.DivFixedSize(value=6)
+                    )
+                )
+            )
+        )
+    ]
+)
+
+```
+
+This example might be serialised like this:
+
+```python
+import json
+
+print(json.dumps(slider.dict(), indent=1))
+# {
+#  "log_id": "sample_card",
+#  "states": [
+#   {
+#    "div": {
+#     "type": "slider",
+#     "max_value": 10,
+#     "min_value": 1,
+#     "thumb_style": {
+#      "type": "shape_drawable",
+#      "color": "#00b300",
+#      "shape": {
+#       "type": "rounded_rectangle",
+#       "corner_radius": {
+#        "type": "fixed",
+#        "value": 100
+#       },
+#       "item_height": {
+#        "type": "fixed",
+#        "value": 32
+#       },
+#       "item_width": {
+#        "type": "fixed",
+#        "value": 32
+#       }
+#      },
+#      "stroke": {
+#       "color": "#ffffff",
+#       "width": 3
+#      }
+#     },
+#     "track_active_style": {
+#      "type": "shape_drawable",
+#      "color": "#00b300",
+#      "shape": {
+#       "type": "rounded_rectangle",
+#       "item_height": {
+#        "type": "fixed",
+#        "value": 6
+#       }
+#      }
+#     },
+#     "track_inactive_style": {
+#      "type": "shape_drawable",
+#      "color": "#20000000",
+#      "shape": {
+#       "type": "rounded_rectangle",
+#       "item_height": {
+#        "type": "fixed",
+#        "value": 6
+#       }
+#      }
+#     },
+#     "width": {
+#      "type": "match_parent"
+#     }
+#    },
+#    "state_id": 0
+#   }
+#  ]
+# }
+```
+
+Templating and DRY
+------------------
+
+Of course, manually building blocks from your code every time is boring. 
+So, the first idea is to move the initialization of DivKit objects 
+into functions.
+
+```python
+# Naive DRY example which strictly non-recommended
+import pydivkit as dk
+
+
+def get_size(value: int = 32) -> dk.DivFixedSize:
+    return dk.DivFixedSize(value=value)
+
+
+def get_shape() -> dk.DivShape:
+    return dk.DivShape(
+        item_width=get_size(),
+        item_height=get_size(),
+        corner_radius=get_size(100)
+    )
+
+    
+slider_shape = get_shape()
+
+slider = dk.DivData(
+    log_id="sample_card",
+    states=[
+        dk.DivDataState(
+            # other arguments
+            div=dk.DivSlider(
+                thumb_style=dk.DivShapeDrawable(
+                    shape=slider_shape,
+                    # other arguments
+                ),
+                # other arguments
+            )
+        )
+    ]
+)
+```
+
+Looks a little better, but this approach doesn't scale well. To simplify layout 
+and save traffic, DivKit has templates. This is a way to layout similar elements
+without having to declare the complete json, but just declare a template and use
+this many times in similar items.
+
+**PyDivKit supports defining templates through the inheritance.**
+
+Let's define an example card:
+
+```python
+import json
+
+import pydivkit as dk
+
+
+class CategoriesItem(dk.DivContainer):
+    """
+    Class inherited from dk.DivContainer will have a template
+    """
+
+    # Special object for mark this fields a DivKit field in template
+    icon_url: str = dk.Field()
+    text: str = dk.Field()
+
+    # Set defaults layout for in the template
+    width = dk.DivWrapContentSize()
+    background = [dk.DivSolidBackground(color="#f0f0f0")]
+    content_alignment_vertical = dk.DivAlignmentVertical.CENTER
+    orientation = dk.DivContainerOrientation.HORIZONTAL
+    paddings = dk.DivEdgeInsets(left=12, right=12, top=10, bottom=10)
+    border = dk.DivBorder(corner_radius=12)
+    items = [
+        dk.DivImage(
+            width=dk.DivFixedSize(value=20),
+            height=dk.DivFixedSize(value=20),
+            margins=dk.DivEdgeInsets(right=6),
+
+            # Special object Ref it's a reference for Field property
+            image_url=dk.Ref(icon_url),
+        ),
+        dk.DivText(
+            width=dk.DivWrapContentSize(),
+            max_lines=1,
+
+            # Special object Ref it's a reference for Field property
+            text=dk.Ref(text),
+        ),
+    ]
+
+
+BASE_URL = "https://leonardo.edadeal.io/dyn/re/segments/level1/96"
+
+
+# So after class definition you might use all the `Field` marked property
+# names as an argument.
+
+gallery = dk.DivGallery(
+    items=[
+        CategoriesItem(
+            text="Food", icon_url=f"{BASE_URL}/food.png",
+        ),
+        CategoriesItem(
+            text="Alcohol", icon_url=f"{BASE_URL}/alcohol.png",
+        ),
+        CategoriesItem(
+            text="Household", icon_url=f"{BASE_URL}/household.png",
+        ),
+    ]
+)
+
+print(json.dumps(dk.make_div(gallery), indent=1, ensure_ascii=False))
+# {
+#  "templates": {
+#   "__main__.CategoriesItem": {
+#    "type": "container",
+#    "background": [
+#     {
+#      "type": "solid",
+#      "color": "#f0f0f0"
+#     }
+#    ],
+#    "border": {
+#     "corner_radius": 12
+#    },
+#    "content_alignment_vertical": "center",
+#    "items": [
+#     {
+#      "type": "image",
+#      "height": {
+#       "type": "fixed",
+#       "value": 20
+#      },
+#      "$image_url": "icon_url",
+#      "margins": {
+#       "right": 6
+#      },
+#      "width": {
+#       "type": "fixed",
+#       "value": 20
+#      }
+#     },
+#     {
+#      "type": "text",
+#      "max_lines": 1,
+#      "$text": "text",
+#      "width": {
+#       "type": "wrap_content"
+#      }
+#     }
+#    ],
+#    "orientation": "horizontal",
+#    "paddings": {
+#     "bottom": 10,
+#     "left": 12,
+#     "right": 12,
+#     "top": 10
+#    },
+#    "width": {
+#     "type": "wrap_content"
+#    }
+#   }
+#  },
+#  "card": {
+#   "log_id": "card",
+#   "states": [
+#    {
+#     "div": {
+#      "type": "gallery",
+#      "items": [
+#       {
+#        "type": "__main__.CategoriesItem",
+#        "icon_url": "https://leonardo.edadeal.io/dyn/re/segments/level1/96/food.png",
+#        "text": "Food"
+#       },
+#       {
+#        "type": "__main__.CategoriesItem",
+#        "icon_url": "https://leonardo.edadeal.io/dyn/re/segments/level1/96/alcohol.png",
+#        "text": "Alcohol"
+#       },
+#       {
+#        "type": "__main__.CategoriesItem",
+#        "icon_url": "https://leonardo.edadeal.io/dyn/re/segments/level1/96/household.png",
+#        "text": "Household"
+#       }
+#      ]
+#     },
+#     "state_id": 0
+#    }
+#   ]
+#  }
+# }
+```
+
+Template names
+--------------
+
+By default, templates are collecting by the metaclass into shared storage when 
+the class is declaring at import time, and have the 
+format `{module_name}.{class_name}`.
+
+The following example, sure will not occur in the wild, shows a warning if 
+suddenly the names of the classes, and hence the templates, conflict.
+
+```python
+import pydivkit as dk
+
+
+class MyTemplate(dk.DivContainer):
+    width = dk.DivWrapContentSize()
+
+
+class MyTemplate(dk.DivContainer):
+    pass
+
+# RuntimeWarning: Template 'test.MyTemplate' already defined in 
+# <class 'test.MyTemplate'> and will be replaced to <class 'test.MyTemplate'>
+```
+
+Also, if you do not want to show the structure of your project to the outside, 
+or for some reason you need to make the example above clean, you can rename the
+template by declaring a special attribute `__template_name__`
+
+```python
+import pydivkit as dk
+
+
+class MyTemplate(dk.DivContainer):
+    width = dk.DivWrapContentSize()
+
+print(MyTemplate.template_name)
+# >>> test.MyTemplate
+
+class MyTemplate(dk.DivContainer):
+    __template_name__ = "MyTemplate2"
+
+print(MyTemplate.template_name)
+# >>> MyTemplate2
+```
 
-setup(**setup_kwargs)
```

