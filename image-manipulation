import cv2

path = "C:/Users/Cast/Documents/imagens/4x17x198.bmp"
img = cv2.imread(path)

imgGray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
imgBlur = cv2.GaussianBlur(imgGray,(7,7),1)

cv2.imshow("Original",img)
cv2.imshow("Original",imgGray)
cv2.imshow("Original",imgBlur)
cv2.waitKey(0)
----------------------------------
import cv2
import numpy as np

img = np.zeros((512,512),np.uint8) #cria uma imagem de cor preta
print(img.shape)
#img[:] = 255,0,0. modifica a imagem para azul

cv2.line(img(0,0),(300,300),(0,255,0),3)#Cria uma linha diagonal verde na imagem
#(img.shape[1],img.shape[0])cria uma linha diagonal até o fim da imagem
cv2.rectangle(img,(0,0),(250,350),(0,0,255),2)#cria um retangulo
cv2.circle(img,(400,50),30,(255,255,0),5)#cria um circulo
cv2.putText(img,"OPENCV",(300,100),cv2.FONT_HERSHEY_COMPLEX,1,(0,150,0),1)#cria um texto(opencv)


cv2.imshow("Image", img)

cv2.waitKey(0)
