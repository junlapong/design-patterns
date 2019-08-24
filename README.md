# Design patterns

> **Note**  
1.ตัว pattern ที่เหลือโอกาสใช้มันค่อนข้างต่ำมากถ้ามีเวลาผมจะมาทำต่อนะครับ  
2.หากใครต้องการช่วยทำต่อหรือแก้ไขต่างๆ fork ออกไปแล้วทำ pull request เข้ามาจะเป็นพระคุณมากครับ  
3.หากอ่านแล้วสงสัย หรือ อธิบายตรงไหนผิด ตั้งเป็น Issue ทิ้งไว้ก็ได้ เดี๋ยวจะกลับมาตอบขอรับ  
4.เจ้าหนังสือด้านล่างผมไม่ได้เขียน แต่ผมเอารูปเขามาใช้เลยใส่เครดิตให้เขาเฉยๆ จะซื้อไม่ซื้อก็แล้วแต่ศรัทธาเลยละกัน ส่วนตัวผมว่าอ่านแล้วก็สนุกดี  

## มันคืออะไร ?
**Design patterns** เป็นแนวคิดในการแก้ปัญหาที่เราเจอบ่อยๆในการออกแบบซอฟต์แวร์ ซึ่งถ้าเรามี `ปัญหา` แล้วปัญหานั้นมีลักษณะตรงกับ `pattern` ไหนก็ตาม เราก็จะสามารถนำแนวคิดของ pattern นั้นๆไปแก้ปัญหาของเราได้เลย  

**Pattern** แต่ละตัวจะเป็นแค่ `แนวคิดในการแก้ไขปัญหา` เท่านั้น ซึ่งมันไม่ได้บอกชัดเจนว่าเราต้องมีทำอะไรบ้างเพื่อจะแก้ปัญหาที่เจอ ดังนั้นวิธีการแก้ปัญหาที่เจอจะขึ้นกับการตัดสินใจของ developer เอง

## 👍 ข้อดี
* เมื่อเกิดปัญหาในการออกแบบซอฟต์แวร์ สามารเอา pattern มาแก้ปัญหาได้เลย
* สามารถรับมือเมื่อเจอกับ business requirement ที่ซับซ้อนได้
* ลดการเกิด coupling, โค้ดยืดหยุ่นขึ้น, โค้ดนำกลับมาใช้ใหม่ได้

## 👎 ข้อเสีย
* Design pattern แต่ละตัวไม่ได้เข้าใจง่ายสำหรับ developer มือใหม่
* Developer ส่วนใหญ่จะนำ design pattern ไปใช้เลย โดยไม่ได้ชั่งน้ำหนักก่อนใช้ให้ดีก่อน ทำให้โค้ดมีความซับซ้อนเพิ่มขึ้นโดยไม่จำเป็น

> **คำเตือน**  
การนำ design pattern ไปใช้ไม่ใช่เรื่องเท่ เพราะมันมี cost (memory, processing overhead & complexity) ของมันค่อนข้างสูง ดังนั้นก่อนใช้ให้ **ชั่งน้ำหนัก ข้อดี/ข้อเสีย** ให้ดีก่อน ไม่งั้นโค้ดจะทำงานได้แต่ maintenance ยากขึ้นโดยใช่เหตุ `ดังนั้นอย่าเมากาวแล้วตะบี้ตะบันเอา pattern ไปใช้เลยตลอดเวลา` (อาตตามาเตือนแล้วนะ)  

## กลุ่มของ patterns ต่างๆ
Pattern ทั้งหมดถูกแบ่งออกเป็น 3 กลุ่ม ตามวัตถุประสงค์ในการแก้ไขปัญหาของมัน โดยแต่ละกลุ่มจะช่วยให้โค้ดนั้น ลดการเกิด coupling, มีความยืดหยุ่นขึ้นและนำกลับมาใช้ใหม่ได้

* **Creational patterns** - ช่วยในการออกแบบเมื่อจะสร้าง object ต่างๆ
  * [Abstract factory pattern](AbstractFactory.md)
  * [Builder pattern](Builder.md)
  * [Factory method pattern](FactoryMethod.md)
  * [Prototype pattern](Prototype.md)
  * [Singleton pattern](Singleton.md)

* **Structural patterns** - ช่วยในการออกแบบโครงสร้างของ class ต่างๆ
  * [Adapter pattern](Adapter.md)
  * [Bridge pattern](Bridge.md)
  * Composite pattern
  * [Decorator pattern](Decorator.md)
  * [Facade pattern](Facade.md)
  * Flyweight pattern
  * [Proxy pattern](Proxy.md)

* **Behavioral patterns** - ช่วยในการออกแบบให้ class ต่างๆทำงานร่วมกัน
  * [Chain of responsibility pattern](ChainOfResponsibility.md)
  * [Command pattern](Command.md)
  * Interpreter pattern
  * [Iterator pattern](Iterator.md)
  * [Mediator pattern](Mediator.md)
  * [Memento pattern](Memento.md)
  * [Observer pattern](Observer.md)
  * [State pattern](State.md)
  * [Strategy pattern](Strategy.md)
  * [Template Method pattern](TemplateMethod.md)
  * [Visitor pattern](Visitor.md)

# Credit
https://refactoring.guru  
You can buy his book by click the image below.  
[![img](https://refactoring.guru/images/patterns/book/web-cover-en.png)](https://refactoring.guru/design-patterns/book#buy-now)  
