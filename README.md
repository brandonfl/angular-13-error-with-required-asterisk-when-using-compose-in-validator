## Required asterisk when using required validator dont work with Validator.compose


The feature introduced by https://github.com/angular/components/pull/23362 seems to dont work with Validator.compose feature

### Reproduction
StackBlitz : https://stackblitz.com/edit/angular-mat-input-lpt6la?file=src/app/app.component.html

### Steps to reproduce:

Create a mat-form-field input with formControlName that have a Validators.required
Do the same with a Validators.compose that contain a Validators.required
Expected Behavior
In the 2 mat-form-field input you sould have the *

### Actual Behavior
You only get it into the one not having Validators.compose

![image](https://github.com/brandonfl/angular-13-error-with-required-asterisk-when-using-compose-in-validator/blob/img/required-with-compose.png?raw=true)
