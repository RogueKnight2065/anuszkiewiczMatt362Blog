# Matt Anuszkiewicz CSCI 362 Blog

## August 22nd, 2019

### HW0: Introduction

My name is Matt Anuszkiewicz. I am a computer science student at the College of Charleston.

This blog is about my CSCI 362 Software Engineering course. 


### HW1: Chapter 1

**1.3.** What are four important attributes that all professional software should possess? Suggest four other attributes that may sometimes be significant.
    
    - Acceptability
    - Dependability and Security
    - Efficiency
    - Maintainability
    
    - Heterogeneity
    - Able to adapt to changing social and business needs 
    - Security and trust
    - Scale
    
**1.8.** Discuss whether professional engineers should be licensed in the same way as doctors and lawyers.

   Professional engineers should be licensed because some if not all the technology they make could have the possibility of killing or effecting human society in some way.

**1.9.** For each of the clauses in the ACM/IEEE Code of Ethics, propose an appropriate example that illustrates that clause. 
    
    - Public: Shall act with public interest in mind.
    - Client and Employer: Shall act in a manner that holds the interests of the client, employer, and public.
    - Product: Shall ensure that the product is high quality and can be modified.
    - Judgement: Shall maintain integrity and independence of their judgement. 
    - Management: Leaders shall promote ethical practices and manage software development and maintain.
    - Profession: Shall advance the integrity and reputation of the profession with public interest.
    - Colleagues: Shall be fair to and support colleagues of all ranks.
    - Self: Shall participate in lifelong learning regarding the practice of the profession. 
    

**1.10.** To help counter terrorism, many countries are planning or have developed computer systems that track large numbers of their citizens and their actions. Clearly, this has privacy implications. Discuss the ethics of working on the development of this type of system.

   It is understandable that most countries would consider making computer systems to track and analyze citizens of their own country. The amount of intelligence needed to track down and eliminate the threat of terrorism is extremely large, cumbersome, and extremely complex. The issue is that most objectives of terrorism is to cause as much havac as possible and to strike fear in a specific group of people. The other issue is that terrorism is not a uniform casue, anyone could be a terrorist. However invading the privacy of everyone to see if they are a terrorist is extremely invasive and can cause worse consiquenses. Tracking movements is fine even if the data is streaming though military satilites like GPS but tracking habbits and puchuses without a warrent is illigel inside the U.S and we should hold other countries accountable. Now a day most people give the world their info so they are easy to track, but tracking everything they do without a warrent is unethical.  




## August 27th, 2019
### HW2: Responces


### HW3: Chapter 10

**10.6.** Explain why it is reasonable to assume that the use of dependable processes will lead to the creation of dependable software?

   Dependencys are everywhere, where something relays on the something else to complete its job. It is ok to have software that is dependent on some aspect, like making a tool for a specific application. However the software should be able to operate on its own if need be.
   If software is entirely dependent then when the software that is being relayed on crashes, not supported anymore, or updates the software that was made as a dependent would be useless. If the software is independent it will have more modularity and would be able to adapt to the changing software without engineer intervention.  


**10.10.** It been suggested that the need for regulation inhibits innovation and that regulators force the use of older methods of systems development that have been used on other systems. Disscudd weather or not you think this is true and the desirability of regulators imposing their views on what methods should be used.

   There is an old saying "If it ain't broke, don't fix it." This saying was taught to me by my father, he used to say it when we had to fix something or if something just flowed right. Sometimes it seems this saying is taking to literally. Polocy and reglation makers when it comes to technology and systems would take that saying to litterally. They not wanting people to change the way software is made or designined, not willing to think outside of the box. 
   One of the main problems of keeping regulations and using older methods is that those methods and systems might already be compromised in security for example a zero day. A zero day is an exploit found in software when it was originally made. 
   Regulation also stunts the growth of innivation. Not allowing designers to think outside of the box and outside of scope to complete a project that might yeild a better solution, will stunt the growth of innivation. 



## August 29th, 2019
### HW 4: Chapter 11 & 12

## September 5th, 2019
### HW6: Chapter 4

**4.5** Using the technique suggested here, where natural language descriptions are presented in a standard format, write plausible user requirements for the following functions: An unnattended petrol (gas) pump system that includes a credit card reader. The customer swipes the card through the reader, then specifies the amount of fuel required.  The fuel is delivered and the customer's account debited. The cash-dispensing function in a bank ATM. In an Internet banking system, a facility that allows customers to transfer funds from one account held with the bank to another account with the same bank.
   *Petrol Pump System:*
    Function: Delivers the correct amount of fuel.  Obtains the correct amount of money.
    Description: Reads the customers card and the amount of fuel, then delivers the correct amount of fuel, as entered by the customer, and debits the customers acount based on the cost of the fuel.
    Inputs: User account information, amount of fuel
    Source: Customers card, card reader, user specified amount
    Outputs: Fuel, reciept
    Action: Outputs n amount of fuel, if n is greater than 0.  Calculates cost per gallon (n * cost).  Subtracts cost amount from user account.  
    Requires: Card reader, input amount from user.
    Precondition: The fuel reservoir contains amount of fuel needed.  The card reader is functioning.
    Postcondition: All information is cleared.
    Side Effects: N/a
    
  *Cash reader:*
    Function: Dispenses the correct amount of money.
    Description: Reads in customer's account information off of card and customer passes the secuity pin.  Takes input from user on how much money is required.  Dispenses the correct amount of money.
    Inputs: User account information, amount of money, secuity pin
    Source: Customers card, card reader, user specified amount, secuity pin
    Outputs: Cash
    Action: Reads user card, pin input and input for money.  Outputs amount of cash specified, if account is greater than zero.  Deducts the amount from the user's account.
    Requires: Card reader, input amount from user, pin reader.
    Precondition: The atm contains the max amount of cash allowed to be deposited.
    Postcondition: All information is cleared.
    Side Effects: N/a
    
  *Internest Banking Transfer:*
    Function: Subtracts correct amount of money from sender's account and adds that amount to reciever's account.
    Description: Obtains user data from sender on how much money is to be transferred and who to transfer to.  Subtracts given amount from that account.  Adds the balance to the reciever's account
    Inputs: User's acount information, amount to be transferred, reciever's information
    Source: User specified
    Outputs: Negative from sender, positive to reciever
    Action: Gets user information from sender and transfers correct amount of money from one account to the other.
    Requires: Input from user.
    Precondition: The user is logged onto the online bank system.  The sender has the reciever's information.
    Postcondition: All information is cleared.
    Side Effects: N/a
  
**4.6** Suggest how an engineer responsible for drawing up a system requirements specifications might keep track of the relationships between functional and non-functional requirements.

An engineer is repsonsible for the system and it's requirements. The engineer could draw up or write out the system requirements and which parts or fuctional and which parts aren't. 

**4.7** Using your knowledge of how an ATM is used, develop a set of use cases that could serve as a basis for understanding the requirements for an ATM system.

- User wants to view account info and amounts
- User wants to widthdraw cash
- User wants to transfer money to different accounts
- User want to deposit check or cash

## September 10th, 2019
### HW8: Chapter 2

**2.1** Suggest the most appropriate generic software process model that might be used as a basis for managing the development of the following systems. Explain your answer according to the type of system being developed.

Developing software for an ECU in a car, mainly involving the ABS, traction, and stablity controls. It can be show that these could of been devoloped using a waterfall techenque. The reasoning is that if something happen like slamming on brakes or slidding across the road the ECU detects the movement of the car and uses its systems to control the movement of the car to make it safe. For ABS the brakes are applied at a pumping rate until the vehichle is at a stopping point. For stablity and traction control the ECU could pump the brakes until car stops sliding, or cut the throatle until the car catches tration. All 3 of these systems I suggest using the waterfall method due to the safety requirements and the ECU needes specific input to turn these on properly without damaging the car or driver. 

## September 12th, 2019
### HW10: Chapter 5

**5.3** You have been asked to develop a system that will help with planning large-scale events and parties such as weddings, graduation celebrations, and birthday parties.  Using an activity diagram, model the process context for such a system that shows the activities involved in planning a party (booking a venue, organizing invitations, etc.) and the system elements that might be used at each stage.

**5.5** Develop a sequence diagram showing the interactions involved when a student registers for a course in a university.  Courses may have limited enrollment, so the registration process must include checks that places are available.  Assume that the student accesses an electronic course catalog to find out about available courses.

**5.7** Based on your experience with a blank ATM, draw an activity that models the data processing involved when a customer withdraws cash from the machine.

**5.8** Draw a sequence diagram for the same system.  Explain why you might want to develop both activity and sequence diagrams when modeling the behavior of a system.

## September 17th, 2019
### HW:11 Chapter 6

**6.4** Draw diagrams showing a conceptual view and a process view of the architectures of the following systems:

A ticket machine used by passengers at a railway station.
A computer-controlled video conferencing system that allows video, audio, and computer data to be visible to several participants at the same time.
A robot floor-cleaner that is intended to clean relatively clear spaces such as corridors.  The cleaner must be able to sense walls and other obstructions.

## September 24th, 2019
### HW13: Chapter 8

**8.7** Write a scenario that could be used to help design tests for the wilderness weather station system.

Depending on the wilderness you are putting the sensors. However if there were multiple stations around the world detecting different places, a system should be built that has easy to read parameters. The system should require GPS location, tempature, altitude, air pressure and huminity. Testing in local area should be done first. If needing extra seners, it is suggested to do radiation if in hazardish areas. 

**8.10** A common approach to system testing is to test the system until the testing budget is exhausted and then deliver the system to customers. Discuss the ethics of this approach for systems that are delivered to external customers.

It is smart for the company to allocate funds for system testing only. The issue is if the allocated funds are to small to test the whole project. Another issue could be that there was so much money in the testing that the project is taking forever to come out. Also there could be the thought that if just the system is being test from the budget what about its componets and the security of the entire system. 

## October 3rd, 2019
### HW16: Chapter 9

**9.8** Briefly describe the three main types of software maintenance. Why is it sometimes difficult to distinguish between them?

Fault repairs, envirormental adaptions, and fuctionality additions are the 3 different types of software maintenance. It is hard to tell the difference between them because they are often apart of the same issue and are often worked on at the same time. Debugging these faults is done usually all at once. If changing environments it is possible to introduce new bugs to the process. This more debugging needs to happen. 

**9.10** Do software engineers have a professional responsibility to develop code that can be easily maintained even if their employer does not explicitly request it?

I would assume yes they do have a responseablity to the maintainablity to their code. However this seems to not be in practice from some of the code I have seen. Most of the documentation is not kept well or there is some weird fault that is hard coded into the system. Ethically I think that it should be their duty to make proper documentation and make their software easy to maintain. 

## October 1st, 2019
### HW15: Chapter 15

**15.10** The reuse of software raises a number of copyright and intellectual property issues. If a customer pays a software contractor to develop a system, who has the right to reuse the developed code? Does the software contractor have the right to use that code as a basis for a generic component? What payment mechanisms might be used to reimburse providers of reusable components? Discuss these issues and other ethical issues associated with the reuse of software.

I think it is a possible to use the developed code for a project. However their should be some crediation to the developer of the original software. There should be payment to the original developer or at least a certain percentage to the original developer. Also the customer should know that you are using some one else's code. Otherwise the company, you, or them could get sued.

## October 8th, 2019
### HW17-A: Chapter 16
**16.9** Design the interfaces of components that might be used in a system for an emergency control room. You should design interfaces for a call-logging components that record calls made, and a vehicle discovery component that, given a post code(zip code) and an incident type, finds the nearest suitable vehicle to be dispatched to the incident. 
*Call logger*
```
{
Input: callData, dispatcherData, callerData
Output: callReport, sendDispatch, startCall, endCall, listAll
Exceptions: Caller misusing 911 sevirces
}
```
*Vehicle Discoverer*
```
{
Input: postCode, incidentType, currentVehicleLocation
Output: dispatchEmergencyVehicle
Exceptions: denigned service
}
```
The Vehicle Discoverer interface's inputs are made from the callReport from the call logger.

## October 10th, 2019 
### HW17-B: Chapter 17

**17.10** Your company wishes to move from using desktop application to accessing the same functionality remotely as services. Identify three risks that might arise and suggest how these risks may be reduced.
    Remote access has its own security problems not to mention the latency and morale of the teams. Remoting in to a site runs the risk of someone or something tracking your traffic and possible could hijack your connection, or listen to all of the traffic back to the host computer. This is a massive risk to the security of the company, client, and the users of the products. This risk can be midagated by requiring a VPN on all computers that access the company, SSH remote servers with key autherization, and to have employees who are security conscious. 
    When remote connecting to something there is always travel time from the client computer to host. Having this latency issue will cause possible errors or bug in the code that the company is working on. The only way this issue can be fixed or midigated is to have a robust network of servers to support the traffic coming through. 
    While assosiates are at home it is possible that they could lose connection with the team they are working with. In return this might decrease productivity and might cause issues with the client. This can be fixed by having the employees come in for meetings every relaese. 


## October 15th, 2019
### HW18: Charpter 18

**18.4** Define an interface specification for the Currency Converter and Check credit rating services shown in Figure 18.7.
*Currency Converter*
```
{
//Convert
Input: Amount(double), recivedCurrency(string), exchangeToCurrency(string)
Output: convertedAmount(double) 
Exceptions: Invalid Currency, User misentry

//exchangeRate
Input: recivedCurrency(string), exchangeToCurrency(string)
Output: exchangeRate(double)
Exceptions: Invalid Currency, User misentry
}
```
*Check Credit Rating*
```
{
//creditHistory
Input: id(int), creditCompany(string)
Output: report (string)
Exceptions: Invalid Entry, Account does not exist, Invalid company, no history for ID. 

//creditRating
Input: id(int), creditCompany(string)
Output: creditScore(int), analysis(string)
Exceptions: Invalid Entry, Account does not exist, Invalid company
}
```


## October 22nd, 2019
### HW19: Chapter 19

**19.3** Why is it impossible to infer the emergent properties of a complex system from the properties of the system components?
   
   A system is not just a singular thing, they are normally a collection of subsystems that also has the emergent properties of the connected subsystems and the integration of the subsystems. For complex systems the complexities mostly appear in the critial relationships between the componets of the system. The emergent properties involve the system as a whole, it is not an isolated part of the system. The same properties of reliability, security, and preformance come from not just the individual componets or the system as a whole. They emerge from how the systems and its componets work together and how the complex relationship is managed. For these reasons is why it is impossible to infer that emergent properties of a complex system from its properties of the system componets. 


## October 24th, 2019
### HW20: Chapter 20

**20.10** You work for a software company that has developed a system that provides information about consumers and that is used within a SoS by a number of other retail businesses. They pay you for the service used. Discuss the ethics of changing the system interfaces without notice to coerce userd into paying higher charges. Consider this question from the point of view of the company's employees, customers, and shareholders.

   There is an ethical issue when it comes to raising the prices toward a customer. However this already occues in the work place. For example when the bank charges overdraft fees or anyother fees that are charged to the customer. This has an advatage on the company giving out the fees because the company can charge whatever they like. From the shareholders prespective charging more money to the customer for using their service is fine. They personally do not have to pay and it gains them more money. From the aspect of the employee it might feel scummy for the fact they are charging the customer more money, however it works in their benifit. 
   
## Ocotber 29th, 2019
### HW21: Team Progress

From today, our team is doing well. We feel that we are ahead of schedule when it comes to the deliverables. We just starting with the code injection part. Dr. Bowering gave us some good feedback on our last deliverable. He pointed out how he would like our project should be running and how to audimate the testcase generation process. I think Benji really wants to do something along the lines of testcase audimation. 
    
## October 31st, 2019
### HW22: Chapter 21

**21.4** Explain why an object-oriented approach to software development may not be suitable for real-time systems.

Object-oriented approach to software development may not be the best practice for real-time systems. Real-time systems need to be updated constantly and need to re responcive immiately. Object oriented is slower than most other approachs to software and takes up more memory. A real-time system need the memory to store it's data and the speed to be up to date. 

## November 3rd, 2019
### HW23: Chapter 22

**22.6** Fixed-price contracts, where the contractor bids a fixed price to complete
a system development, may be used to move project risk from client to
contractor.  If anything goes wrong, the contractor has to pay.  Suggest
how the use of such contracts may increase the likelihood that project
risks will arise.

Having a fixed price to a project could become an issue in the long run. The project that is being worked on could be extremely underpriced from the assets used or if there is an extreme delay. It could also mess with the quality of the project itself. Some people would say it is worth that ammount "ok that is what I will make that is it." It could also cause an issue for a customer if that fixed price is way over the ammount that the software is worth. If the project is bidded on the it is possible that the bid was too low to meet the specifications for the project. 

## November 7th, 2019
### HW24: Chapter 23

**23.6** Figure 23.14 shows the task duration for software project activities.  Assume that a serious, unanticipated setback occurs, and instead of taking 10 days, task T5 takes 40 days.  Draw up new bar charts showing how the project might be reorganized.

## November 12th, 2019
### HW25: Team Progress

We are doing well, felt alittle behind. Benji decided to focus on the testcase audimation. We found some spots to implement our code injections. The wiki is up to date but our files are everywhere. 

## Novemeber 16th, 2019
### Chapter 24

**24.6** Explain why program inspections are an effective technique for discovering errors in a program. What types of errors are unlikely to be discovered through inspections?

Program inspectors are useful for their ablity to look at code and fix it. Normally the inspector is looking for errors and general debugging. This can be helpful because the inspector hasn't been staring at the code for hours and has no bias to the code itself. They are unlikely to find errors in the whole system or component errors. 


## Novemeber 19th, 2019
### HW27: Chapter 25

**25.10** Describe five factors that engineers should take into account during the process of building a release of a large software system.

1. Documentation: It is neeeded to document everything and breifily decribing what the program does in the system. If the docuemtation is kept up it is easier to read and maintain. 
2. Branching and merging: Branching and merging your software might cause some issue with updating the software and might cause errors. 
3. Testing: Test everything and every part of the system. Testing will insure some integraty of the system.
4. Competition: Sence it takes awhile to make software competition can pop up and might be a competitor to the company or whom ever was making the system.
5. Availibiliity: The system must be able to work on mulitple systems, the software must be tested and flxible. 
