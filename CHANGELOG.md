# Changelog

## v1.3.3 - 2026-04-23
### Fixes
- Removed orphaned Windows Vista entry from `package.json` (theme file was never created)
- Fixed CHANGELOG version typo (`v1,2,7` → `v1.2.7`)

### Improvements
- **Windows 3.1 Classic**: Added ~34 missing workbench color keys (`input.*`, `menu.*`, `scrollbarSlider.*`, `sideBarSectionHeader.*`, `tab.*`, `editorGroup.*`, and more) and missing markup token scopes (`markup.heading`, `markup.italic`, `markup.bold`, `markup.inline.raw/fenced_code.block`)
- **Windows 98**: Added `activityBarTop.foreground`, `tab.hoverBackground`, `tab.hoverForeground`, `tab.activeModifiedBorder`, `tab.inactiveModifiedBorder`
- **Windows XP Blue**: Added `activityBarTop.foreground`, `menu.background`, `scrollbarSlider.hoverBackground`
- **All light themes**: Added `activityBarTop.foreground` to Windows ME, XP Light, XP Blue, 7, 98, and 3.1 Classic; set to `#616161` on themes with colored activity bars for better contrast when the activity bar is positioned at the top

## v1.3.0 - 2026-03-07
### Fixes
- Fixed JSON syntax error (trailing comma) in Windows XP Blue theme
- Fixed Windows XP Dark incorrectly declared as a light theme (`uiTheme: vs` → `vs-dark`), which was causing white backgrounds throughout the theme
- Fixed `icon.foreground` on all light themes (was `#FFFFFF`, making editor toolbar icons invisible against light backgrounds)
- Fixed `list.inactiveSelectionBackground` on Windows XP Dark (was light gray `#DADADA`, copied from the light variant)

### Improvements
- **Terminal colors**: Added full 16-color ANSI palette (`terminal.ansi*`) to all themes, with colors derived from each theme's own palette
- **Git decorations**: Added `gitDecoration.*` colors to all themes so modified/added/deleted/untracked files are properly colored in the Explorer
- **Diff editor**: Added `diffEditor.*` colors to all themes for inline diff and merge editor views
- **Activity bar**: Added `activityBar.inactiveForeground` to all themes so inactive icons are visible alongside extensions like Claude Code
- **Syntax highlighting**: Added token color scopes missing from all themes — `variable.parameter` (italic), `variable.language` (`this`/`self`), `meta.object-literal.key` (object/JSON keys), `invalid.illegal` (syntax errors)
- **Consistency**: Added missing `badge`, `panelTitle`, and `toolbar` color keys to themes that were lacking them
- **Windows 98 Desert**: Differentiated previously near-identical token colors — comments (olive), strings (amber), constants (burnt orange), keywords (bright gold), functions (teal), types (sage)
- **Windows 98 Eggplant**: Differentiated previously near-identical token colors — comments (muted purple), strings (sage green), constants (gold), keywords (pink-purple), functions (blue-teal), types (sky blue)

## v1.2.7 - 2025-12-24
### Improvements
- Finetuning colors in some Windows XP themes and Windows 7 theme

## v1.2.6 - 2025-07-10
### Improvements
- Better readability for icons in the title section of side bar panels (such as open editors, timeline and outline panel)
### Fix
- Adjusted extension version number in CHANGELOG

## v1.2.5 - 2025-06-12
### New
- 🎨 **Windows 98 Theme Variants**:
  - **Eggplant**: Deep purple theme with sage accents
  - **Desert**: Warm sandy theme using earthy tones
  - **Rainy Day**: Soft blue-gray theme for cloudy days

### Improvements
- 🔄 **Windows ME Theme Update**:
  - Refreshed color scheme
  - Enhanced UI with soft blue accents
  - Added complementary shades for better contrast
  - Improved overall visual harmony

## v1.2.1 - 2025-06-03
### Improvements
- 🖌️ **Better readability for the following :**
  - Selection colors in editor
  -  Active/inactive items in list view (such as `Ctrl+Shift+P` / `Cmd+Shift+P`, or File Explorer)

## v1.2.0 - 2025-05-17
### New
- 🎮 **Windows 3.1 Classic**: Experience the nostalgic look of the original Windows 3.1 with authentic colors and design
- Updated theme documentation with detailed specifications

### Improvements
- 🖥️ **Windows 98 Enhanced**: Major improvements to the Windows 98 theme
  - More authentic system colors (#C0C0C0, #000080, #808080)
  - Enhanced 3D border effects for better authenticity
  - Improved syntax highlighting with more scopes
  - Better contrast and readability
  - Added proper hover states and focus indicators
  - Enhanced markdown support

- 🎨 **Windows XP Themes Overhaul**: Complete refresh of all Windows XP themes
  - Light Theme:
    - Authentic Luna colors and styling
    - Improved contrast and readability
    - Enhanced UI elements consistency
  - Dark Theme:
    - Refined dark mode aesthetics
    - Better color harmony
    - Improved visibility in low-light
  - Blue Theme:
    - Authentic Luna Blue color scheme
    - Enhanced visual hierarchy
    - Refined syntax highlighting
  - Common Improvements:
    - Added proper border effects
    - Enhanced editor customization
    - Improved markdown support
    - Better syntax highlighting scopes
    - Added hover and focus states

- 🌟 **Windows 7 Modernized**:
  - Added authentic Aero-inspired design
  - Implemented Windows 7 signature blue (#2672EC)
  - Enhanced UI with modern flourishes
  - Improved button and input styles
  - Added refined hover effects
  - Better syntax highlighting

- 🔄 **Windows ME Refresh**:
  - Authentic Windows ME colors
  - Enhanced UI element styling
  - Improved 3D border effects
  - Better contrast and readability
  - Refined syntax highlighting
  - Enhanced editor experience

## v1.1.4 - 2025-02-06
### New
- 🟦 **Windows XP Blue** theme

## v1.1.0 - 2024-10-13
### Fixes
- Major adjustments to Windows 98 theme

## v1.0.2 - 2024-06-09
### New
- 🚀 **Windows 7**: Carry the legacy of Windows 7 forward, enhancing your experience with every click.

## v1.0.1 - 2024-05-24
### Fixes
- Minor adjustments

## v1.0.0 - 2024-05-25

### New
- 🎉 Initial release of Retro Windows Themes!
- 🌞 **Windows XP Light**: Bright and colorful theme reminiscent of the XP era.
- 🌚 **Windows XP Dark**: A dark mode version for all your nostalgic night coding.
- 🖥️ **Windows 98**: Relive the classic look of Windows 98.
- 📺 **Windows 3.1**: Go back to the basics with this old-school theme.

### Improvements
- Tweaked colors for better readability and more authentic retro vibes.
- Added cool ASCII art to the README because, why not? 😎

---

Stay tuned for more updates and themes! Have a theme suggestion? Let us know! 🎨🚀
