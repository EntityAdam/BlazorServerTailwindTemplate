# Blazor Server Template

## Add template to Visual Studio 2019

- Download `/TemplateFile/BlazorServerTailwindTemplateV1.zip`
- Copy to `%USERPROFILE%\Documents\Visual Studio 2019\Templates\ProjectTemplates\`

## Tailwind with `gulp` references

> https://chrissainty.com/tailwindcss/
> https://chrissainty.com/integrating-tailwind-css-with-blazor-using-gulp-part-1/
> https://chrissainty.com/integrating-tailwind-css-with-blazor-using-gulp-part-2/

## Build

### Install npm dependencies

```s
npm install gulp-cli -g
```

### Build full CSS files for dev

- Creates source maps
- Plops CSS into `wwwroot/css/`

```s
gulp css:dev
```

### Build minimal CSS for release

- Runs purgecss against html and razor files (You may want to include `.cshtml` if using razor pages)
- Runs cleancss
- Creates source maps
- Plops CSS into `wwwroot/css/`

```s
gulp css:prod
```
