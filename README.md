# bs-stepper FORK

This is a fork of [bs-stepper](https://github.com/Johann-S/bs-stepper), please refer to original repository for documentation / license / support the author.

## About the fork

1. Tested with Bootstrap 5 (also updated in devDependencies)
2. "Step completed" feature added

## "Step completed" feature

Simply expanded logic and CSS to mark completed steps with green color and different icons.

![step completed](/docs/img/step-completed.png)

### How to enable this feature

First, init Stepper class as usual, but add `markCompleted: true` parameter:

```
const stepper1 = new Stepper(document.querySelector('#stepper1'), {
    markCompleted: true,
})
```

Then you have to add `<span class="bs-stepper-circle-secondary">...</span>` inside `.step-trigger` button (check tests/index.html for demo)

```
<div class="step" data-target="#test-l-1">
    <button type="button" class="btn step-trigger">
        <span class="bs-stepper-circle">1</span>
        <span class="bs-stepper-circle-secondary">
        ...
        </span>
        <span class="bs-stepper-label">First step</span>
    </button>
</div>
```

### How to use this fork

TODO