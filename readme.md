# Hugo Sizer

Small python CLI to compute and insert sizes of any routes in a Hugo static website.

## Getting Started

### Prerequisites

This CLI call the [Hugo](https://gohugo.io/installation/) command, you will need to have it in your path

### Installing

This command is available on [PyPI](https://pypi.org/project/hugo-sizer/0.1/), you can install it with :
```
pip install hugo-sizer
```

### Usage

You will need to include in your template an HTML tag with the id `hugo-sizer` and any text inside (ex. `XX`), this text will be replace by the actual size.
A basic usage is :
```html
<div class="floating-size">
    This page download only <span id="hugo-sizer">XX</span> kB.
</div>
```
```css
.floating-size{
    position: fixed;
    top: 0;
    right: 0;
}
```
After installing and generating your site `public` folder, you can run the cli in your Hugo project root directory:
```
hugo-sizer
```


## License

This project is licensed under the [MIT License](LICENSE.md)


