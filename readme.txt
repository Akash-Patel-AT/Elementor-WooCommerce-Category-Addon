=== Advanced Custom CSS for Elementor ===
Contributors: agreem2016
Tags: elementor, custom css, ACCE, responsive design, frontend editor
Requires at least: 7.0
Tested up to: 6.9
Stable tag: 1.0
Requires PHP: 7.4
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Advanced Custom CSS for Elementor.

== Description ==
Advanced Custom CSS for Elementor (ACCE) adds a dedicated Custom CSS section to the **Advanced** tab of every Elementor widget.  
It lets you write clean, widget-scoped CSS using the `selector` keyword and provides separate fields for **Desktop**, **Tablet**, and **Mobile** styling.

No premium version required — works with both Elementor Free and Elementor Pro.

Perfect for users and developers who need fast, responsive CSS control directly inside the Elementor editor.

== Features ==
- Adds a **Custom CSS panel** to all Elementor widgets.
- Separate CSS fields for **Desktop**, **Tablet**, and **Mobile**.
- Supports the `selector` keyword for precise widget-only CSS.
- Uses Elementor's live preview for instant visual updates.
- Breakpoints can be customized with a simple filter.
- Lightweight, fast, and requires no additional settings.

== Installation ==
1. Upload the plugin folder to `/wp-content/plugins/`.
2. Activate the plugin through the **Plugins** screen in WordPress.
3. Open Elementor, select any widget, and go to **Advanced > ACCE Custom CSS**.

== Usage ==
In Elementor editor:

1. Select any widget.
2. Open the **Advanced** tab.
3. Scroll down to **ACCE Custom CSS**.
4. Add your CSS using the `selector` keyword.

Example:

selector {
    background: #f3f3f3;
    border-radius: 8px;
}

== Developer Notes ==
You can override the default breakpoints (Tablet: 768px, Mobile: 425px) using this filter:

add_filter('ACCE_custom_css_breakpoints', function($defaults) {
    return [
        'tablet' => 900,
        'mobile' => 600,
    ];
});

== Frequently Asked Questions ==
= Does it work with Elementor Pro? =
Yes, it works with both Elementor Free and Elementor Pro.

= Does it support live preview? =
Yes. CSS updates appear instantly in Elementor’s visual editor.

== License ==
This plugin is licensed under the GPLv2 or later.

== Changelog ==
= 1.0 =
Initial release with device-based CSS fields and breakpoint customization.

== Upgrade Notice ==
= 1.0 =
First release — adds responsive Custom CSS controls to Elementor widgets.