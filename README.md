# Free Reusable Templ Components
✅ A collection of reusable UI components built with Golang's templ, TailwindCSS, Daisy UI, and Alpine.js.

# Templ
### A language for writing HTML user interfaces in Go.
[https://github.com/a-h/templ](https://github.com/a-h/templ)

## util.go

util.go includes a helper GenerateUniqueKey. I used this dead simple helper to generate a unique ID for most all components.

```
func GenerateUniqueKey(id string) string {
	return id + "-" + strconv.Itoa(rand.Intn(100000))
}
```

## Components

- **alert.templ** - Displays alert messages.
- **breadcrumb.templ** - Navigational breadcrumb.
- **button-link.templ** - Button styled as a link.
- **button-primary.templ** - Primary button style.
- **card.templ** - Card component.
- **checkbox.templ** - Checkbox input.
- **chip.templ** - Chip component.
\
![count up component](https://github.com/tego101/templ_components/blob/main/images/cookie.png)
- **cookies-warning.templ** - Cookies warning message.
\
![count up component](https://github.com/tego101/templ_components/blob/main/images/count-up.gif)
- **count-up.templ** - Count-up animation component.
\
![count up component](https://github.com/tego101/templ_components/blob/main/images/detail-list.png)
- **details.templ** - Details and summary component.
\
![count up component](https://github.com/tego101/templ_components/blob/main/images/input.png)
- **input.templ** - Input field component.
- **loading.templ** - Loading spinner component.
- **modal.templ** - Modal dialog component.
\
![count up component](https://github.com/tego101/templ_components/blob/main/images/progress.png)
- **progress.templ** - Progress bar component.
- **tabs.templ** - Tabbed navigation component.
\
![count up component](https://github.com/tego101/templ_components/blob/main/images/time-line.png)
- **timeline.templ** - Timeline component.

## Usage

All components contain usage details for example here's input.templ:

```
/**
* Text Input Component.
* ======================
* This is a input component that can be used to create text inputs.
*
* @params InputProps
* @author: github.com/tego101 <-> x.com/tegodotdev
* @license: MIT
*
* Usage:
* @components.Input(components.InputProps{
*   Type: "text",
*   Name: "First Name",
*   Placeholder: "Enter your name",
*   Class: "max-w-6xl",
*   HideLabel: true,
* })
 */
```

## Disclaimer

Some components may be unfinished. Contributions and pull requests are welcome to help complete them.

## Usage

Include the desired component in your Golang templ file, and adjust the TailwindCSS classes and Alpine.js behavior as needed.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
