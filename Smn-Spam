from pynput.keyboard import Key, Controller
import time, math

message = input('Gönderilecek Mesaj:')
count = int(input('Gönderilecek Mesaj Sayısı:'))

for i in range(5):
	print(str(5 - i))
	time.sleep(1)

keyboard = Controller()
waitTime = 0.01 * len(message)
def pressKey(key):
	keyboard.press(key)
	keyboard.release(key)

for i in range(count):
	progress = math.floor(i / count * 100)
	keyboard.type(message)
	pressKey(Key.enter)
	time.sleep(waitTime)

print('Gönderildi')

#Samomen
