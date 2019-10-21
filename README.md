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
