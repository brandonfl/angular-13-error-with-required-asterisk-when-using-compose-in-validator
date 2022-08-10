## Required asterisk when using required validator don't work with Validators.compose


The feature introduced by https://github.com/angular/components/pull/23362 seems to don't work with Validators.compose feature

### Reproduction
StackBlitz : https://stackblitz.com/edit/angular-mat-input-lpt6la?file=src/app/app.component.html

### Steps to reproduce:

1. Create a mat-form-field input with formControlName that have a Validators.required

2. Do the same with a Validators.compose that contain a Validators.required

### Expected Behavior
The 2 mat-form-field input you sould have the `*` into the placeholder

### Actual Behavior
The mat-form-field input with Validators.compose have correct validation (get red color if no input) but don't have the `*` into the placeholder

![image](https://github.com/brandonfl/angular-13-error-with-required-asterisk-when-using-compose-in-validator/blob/img/required-with-compose.png?raw=true)

![image](https://github.com/brandonfl/angular-13-error-with-required-asterisk-when-using-compose-in-validator/blob/img/required-validation-with-compose.png?raw=true)
