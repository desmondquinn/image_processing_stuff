import dhash
from PIL import Image

image = Image.open('image3.jpg')
row, col = dhash.dhash_row_col(image)
print(dhash.format_hex(row, col))


#string=('ab9b93ba093f6b01158fa129da6c7c1d')

image1 = Image.open('img11.jpg')          #include image to compare
row, col = dhash.dhash_row_col(image1)
print(dhash.format_hex(row, col))
string1 =(dhash.format_hex(row, col))    

image2 = Image.open('img12.jpg')
row, col = dhash.dhash_row_col(image2)
print(dhash.format_hex(row, col))
string2 =(dhash.format_hex(row, col))


distance=0
for i in range(1,32):							
	if (string1[i] != string2[i]):
		distance += 1
	


if distance<10:
	print('images are similar')
else:
	print('images not similar')
