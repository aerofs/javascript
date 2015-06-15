# Stylesheets tips and references

## CSS reference

* W3Schools: not even once. Try [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS) instead.

* Fun learning tool: [CSS Diner](https://flukeout.github.io/)

## Less reference

* [http://lesscss.org/](http://lesscss.org/)
* Do not nest Less selectors more than four deep. 
* Avoid loops.
* Be aware that Less compiles to CSS; if you use Less in an inefficient way, the compiled CSS file will be horribly bloated with repetitive or unused selectors.

## Twitter Bootstrap 3 reference

* We use Twitter Bootstrap for our websites' grid system as well as a number of built-in components. In the main aerofs repo, the Bootstrap color scheme and some other variables are customized via `aerofs-variables.less`
* [http://getbootstrap.com/](http://getbootstrap.com/)

## Additional tips

* Check out [https://www.aerofs.com/styleguide/](https://www.aerofs.com/styleguide/) for the AeroFS color scheme and common styles on the marketing website.
* Primary button: Use `.btn-primary` only for positive features, e.g. add a user, join a team, etc. Don't use it for negative features like removing users and leaving a team. Use `.btn-default` or `.btn-danger` when appropriate.
* Page title: Use `<h2>` for page titles. Only capitalize the first letter of the entire title.
* Dialog title: Use `<h4>` for all dialog titles. Only capitalize the first letter of the entire title.
* Error Dialog title: Use `.text-error` for dialog titles that indicates errors.
* Button label: Use capital case, e.g. "Delete User", except for long phrases, e.g. "Show me all the things"
* Disable buttons on form submission:
```$('#foo-form').submit(function() {
    setEnabled($("#submit-foo-button"), false);
    return true;
});````
