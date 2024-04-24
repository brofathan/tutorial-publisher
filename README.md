# Reflection

Nama: Emir Mohamad Fathan <br>
NPM: 2206081982 <br>

1. How many data your publlsher program will send to the message broker in one 
run?

Ada 5 data yang publisher send ke message broker.

2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber 
program, what does it mean?

URL tersebut, yang ada pada subscriber program, juga ada pada publisher program, karena kedua program terhubung ke AMQP broker yang sama yang berjalan di local machine. Hal ini memungkinkan kedua program berkomunikasi satu sama lain.

<br>
<hr>
<br>

- Screen of running RabbitMQ
![image](https://github.com/brofathan/tutorial-publisher/assets/45114836/c36d4bfa-4f2f-40e9-91b0-94029d97132c)

- Console screen of cargo run
![image](https://github.com/brofathan/tutorial-publisher/assets/45114836/268e78d5-3b58-4d33-b0ce-c0e5e1727989)
(Publisher program mengirimkan data ke message queue, mengirim dan memprosesnya, Lalu ia mengembalikan console log seperti ini.)

- Screen of spikes on RebbitMQ
![image](https://github.com/brofathan/tutorial-publisher/assets/45114836/206a4e47-d54b-4af6-ae4d-b178f5910f70)
(Terjadinya spike karena publisher program mengirimkan data berkali-kali ke message queue, jadi grafik menunjukkan bahwa adanya lonjakan message queue.)
