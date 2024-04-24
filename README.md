# Tutorial-8 
## Fikri Dhiya Ramadhana
## 2206819533
## AdvProg-C

### QnA
1. How many data your publlsher program will send to the message broker in one run?  
publisher program akan mengirimkan lima data (UserCreatedEventMessage) ke broker pesan dalam satu kali jalannya karena adanya lima panggilan ke p.publish_event(...) dalam fungsi main(), masing-masing mengirimkan satu pesan.

2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?  
URL "amqp://guest:guest@localhost:5672" sama dalam kedua program publisher dan subscriber. Ini berarti bahwa kedua program terhubung ke broker AMQP yang sama (RabbitMQ) yang berjalan pada mesin lokal (localhost) di port 5672. Selain itu, mereka menggunakan default credential (guest:guest) untuk melakukan otentikasi dengan broker. Ini memastikan bahwa baik publisher maupun subscriber berkomunikasi melalui instansi broker pesan yang sama.