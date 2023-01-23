import cv2
import pytesseract

#tesseract --version

from pytesseract import Output
pytesseract.pytesseract.tesseract_cmd = r'C:\\Program Files\\Tesseract-OCR\\tesseract.exe'
img = cv2.imread('C:/Users/Cast/AppData/Local/Temp/Rar$DIa6552.46801/6x20x198.bmp')
#img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
#custom_config = r'--oem 3 --psm 6'
#test = pytesseract.image_to_string(img, config=custom_config)
#print(test)
#print(pytesseract.image_to_boxes(img))
#cv2.imshow('Result',img)
#cv2.waitKey(0)



#custom_config = r'--oem 3 --psm 6'
#d = pytesseract.image_to_data(img, output_type=Output.DICT,config= custom_config )
#n_boxes = len(d['level'])
#    (x, y, w, h) = (d['left'][i], d['top'][i], d['width'][i], d['height'][i])
#    cv2.rectangle(img, (x, y), (x + w, y + h), (0, 255, 0), 2)

h, w, c = img.shape
boxes = pytesseract.image_to_boxes(img)
for b in boxes.splitlines():
    b = b.split(' ')
    img = cv2.rectangle(img, (int(b[1]), h - int(b[2])), (int(b[3]), h - int(b[4])), (0, 255, 0), 2)

cv2.imshow('img', img)
cv2.waitKey(0)
