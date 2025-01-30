#  Source of (*MarHex*) PiPy  Package
- ## Quick Start
	#### Install Package:
		pip install marhex
- ## Use Package
	- ###  Server Information
		 ####  Display your Server Network Information :
			 from marhex.ServerInfo.network import display_short_info as net_info
			 net_info()
			 
	- ###  Converters
		#### Convert your Number from English to Persian and vice versa :
			from marhex.Converters.lang_num import english_to_persian, persian_to_english
			english_number =  1234
			persian_number  =  english_to_persian(english_number) # ۱۲۳۴
			reverse_english_number  = persian_to_english(persian_number) # 1234
	- ### Validators
		> #### **Note:**  In all validations, if the input data structure has a problem and is not valid, the associated function returns the appropriate error.
		#### Is characters Persian :
			from marhex.Validators.is_iter import is_persian_char
			english_word = "car"
			persian_word=  "ماشین"
			print(is_persian_char(word))    # False
			print(is_persian_char(persian_word))    # True
		#### Validation & Cleaning Mobile Phone Number :
			from marhex.Validators.mobile_phone_number import validation_and_cleaning
			first_phone = 9925522323
			second_phone = 9925522323
			print(validation_and_cleaning(first_phone)) 
		#### Validation & Cleaning National Code :
			from marhex.Validators.national_code import validation_and_cleaning
			national_code = 4234524235
			print(validation_and_cleaning(national_code))
			
