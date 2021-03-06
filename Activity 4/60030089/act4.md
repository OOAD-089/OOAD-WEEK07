encapsulation
Inheritance
polymorphism

Encapsulation การห่อหุ้ม คือการจำกัดการเข้าถึงข้อมูลบ้างอย่างที่ไม่ต้องการให้ส่วนอื่นรับรู้แต่ให้เข้าถึงผ่านส่วนประสาน(interface hiding)

เป็นคุณสมบัติหนึ่งของการเขียนโปรแกรมเชิงวัตถุ ซึ่งเป็นการกำหนดความสามารถในการเข้าถึงสมาชิกภายในคลาส ไม่ว่าทั้งจากภายนอกและภายในคลาสก็ตาม มันถูกใช้เพื่อทำให้ข้อมูลภายในเป็นความลับและมีความปลอดภัย และง่ายต่อการเขียนโปรแกรม

Encapsulation เป็นแนวคิดที่ได้มาจากในชีวิตจริง ในการเขียนโปรแกรมเชิงวัตถุเรามองทุกอย่างเป็นเหมือนออบเจ็คในโลกจริง ยกตัวอย่างเช่น เมื่อคุณต้องการซื้อตั๋วรถไฟฟ้าที่เครื่องจำหน่ายตั๋วอัตโนมัติ คุณจะต้องใส่เงินเข้าไปในเครื่องและเครื่องจะส่งตั๋วให้กับคุณ ในการทำงานที่จะได้ตั๋วมาให้คุณนั้นมีการทำงานภายในซ่อนอยู่ สิ่งเหล่านั้นเป็นสิ่งที่ถูกปกปิดหรือเราเรียกว่า Encapsulation มันไม่จำเป็นที่คุณจะต้องทราบว่าเครื่องนี้ทำงานยังไง แต่สิ่งที่คุณจะต้องรู้คือการใช้งานเครื่องนี้เพื่อที่จะซื้อตั๋ว

Inheritance การสืบทอดคุณสมบัติ คือการสืบทอดโครงสร้างข้อมูลการดำเนินการ
กฎเกณฑ์ของการทำ inheritance
การทํา Inheritance นั้นเป็นการถ่ายทอดคุณสมบัติทุกอย่างจาก
Superclass ไม่ว่าจะเป็น Attribute หรือ Function แต่มีข ้อควรจําว่า
Visibility ของ Attributes หรือ Functions นั้นมีความสมพันธ์กับการทํา 
Inheritance เสมอนั่นคือ
1. Private Attributes/Functions จะถ่ายทอดมาเป็น Private
Attributes/Functions ของ Subclass แต่สวนที่ Inherit มาจาก Private
Attributes/Functions มายัง Subclass จะไม่สามารถเข ้าถึงได ้โดย Function
ที่มีอยู่ใน Subclass แต่ไม่ได ้มาจากการ Inherit
2. Protected Attributes/Functions ของ Superclass จะถ่ายทอด
มาเป็น Protected Attributes/Functions ของ Subclass อนึ่ง การเข ้าถึง
Attributes และ Functions ของ Subclass ที่เกิดจากการ Inherit ในกรณีนี้
จะทําได ้ โดยผ่าน Function ใดๆ ของ Subclass นั้น โดยไม่คํานึงว่าจะเป็น
Function ที่ได ้มาจากการ Inherit หรือไม่
3. Public Attributes/ Functions จะถ่ายทอดมาเป็ น
Public Attributes/Functions ของ Subclass เสมอ

Polymorphism คือการที่วัตถุที่ต่างกันมีปฎิกริยาตอบสนิงต่อฟังก์ชัน/ข้อความที่ต่างกัน

Polymorphism คือการที่ออบเจ็คสามารถมีได้หลายรูปแบบ ซึ่งเกิดจากการสืบทอดจาก super class และมันยังคงรักษาสภาพและคุณสมบัติของ super class ไว้ เช่น ผู้คนในโลก จะมีทั้งนักกีฬา นักร้อง นักดนตรี ซึ่งมันก็คือการมีหลายรูปแบบทางอาชีพของบุคคล ซึ่งเราสามารถใช้คำว่า บุคคล ในการอ้างถึงคนในอาชีพต่างๆ ได้ ซึ่งเป็นแนวคิดของ polymorphism ในการเขียนโปรแกรม ซึ่งมันความหมายของมันคือการมีได้หลายรูปแบบ

ในการเขียนโปรแกรมเชิงวัตถุ Polymorphism นั้นคือการสร้างออบเจ็คโดยเป็นออบเจ็คที่สร้างมาจากคลาสที่มี Super class เดียวกัน โดยใน Sub class นั้นได้มีการกำหนดการทำงานใหม่ให้กับเมธอดให้ตรงกับวัตถุประสงค์ของคลาสนั้น หรือการ Override method หลังจากนั้นเราสามารถใช้ Super class สำหรับการประกาศตัวแปรของออบเจ็ค (class instance) ที่สร้างออบเจ็คจาก Sub class ได้
