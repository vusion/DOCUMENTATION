# REA

REA is a standard which take advantage of Attributes and CSS Modules to simplify BEM.

All CSS selectors in a component are locally due to CSS Modules. Unlike BEM, you don't need think any naming rules.

## R: Root

As we known, there is only one root node in every Vue component. It is like Block in BEM.

Just use `.root` to mark it. It will be converted to the component's name with a hash subfix.

## E: Element

Other nodes in a component are called `Element`, which is similar to BEM.

Use a simple word related to the usage of this element to mark it, like `head`, `item`, `side`, ...

## A: Attribute

Flags on blocks or elements. Use them to change appearance, behavior or state. It is like Modifier in BEM.

## Example

A `<u-linear-progress>` component:

``` html
<div :class="$style.root">
    <div :class="$style.track">
        <div :class="$style.trail"></div>
    </div>
</div>
```

``` css
.root {
    .track {
        height: 20px;
        background: #eee;
    }

    .trail {
        width: 30%;
        height: 100%;
        background: $brand-primary;
    }
}

.root[color="success"] {
    .trail {
        background: $brand-success;
    }
}

.root[active] {
    .trail {
        animation: ...
    }
}
```
