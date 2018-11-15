# MonthYearPicker
Picker dialog to pick only month and year


just copy paste MonthYearPickerDialog.java to your project along with month_year_picker_dialog.xml and two string resources i.e. R.string.on and R.string.cancel.

To use it, just copy below lines

    MonthYearPickerDialog pickerDialog = new MonthYearPickerDialog();
    pickerDialog.setListener(new DatePickerDialog.OnDateSetListener() {
        @Override
        public void onDateSet(DatePicker datePicker, int year, int month, int i2) {
            Toast.makeText(MainActivity.this, year + "-" + month, Toast.LENGTH_SHORT).show();
        }
    });
    pickerDialog.show(getSupportFragmentManager(), "MonthYearPickerDialog");


![Screenshot](https://i.postimg.cc/59kXgjnd/month-year-picker.png)
