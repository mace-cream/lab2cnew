---
title: Social Game
date: 2018-07-07T17:04:41+06:00
image: images/blog/socialgame.jpg
author: Admin
---

### Introduction

Buildings consume about 40% of the total energy in the US and the cost of a building during the operation period compose more than 80% of its total cost over the whole life-cycle span. Therefore, it is vital to reduce the building operation energy consumption. In current commercial building, there are two kinds of control methods. One is the manually control system. As a matter of fact, the majority of electricity users do not need to pay for the corresponding fees, thus, the real payers cannot manage to persuade them into saving energy. Another is Building Automation and Control System.

![Traditional Building Control](../../../images/blog/soc-trad.jpg)
*Fig. 1: Traditional Building Control*

The approach control and reduce energy by estimating user presences. However, this approach has many problems. Estimation can be inaccurate due to preference changes or non-response. Separation of users and the system separate their usage goals.

In order to solve the above problems, we proposes a social-technical system. We get user involved in the process of energy conservation by energy consumption feedback. Besides sensors, user gives a user preference estimation to control system based on his feeling about energy usage and environment. The control system combines the sensory data and user preference estimation to make the control decision.
![Social Game Rationale](../../../images/blog/soc-infr.jpg)
*Fig. 2: Social Game Rationale*

Social feedback allows user direct influence of systems and aligns goal of users and the system.The game is played between the system and the users. The system will announce a reward scheme for individual user or a group of users if they meet some energy saving requirement, and the users will make the decision whether they participate the game. Below is a figure to illustrate the system logics, where the combination of the game rule maker, the referee, and the reward dispenser is the system.
![Logics of the Social Game](../../../images/blog/soc-sys.jpg)
*Fig.3 Logics of the Social Game*

There are two types of game of interests.

- Individual Game: 
This type of game deals with the personal electricity consumption, aka the cubical energy bill, for example, the PC, desk lamps, phone chargers, etc. The personal electricity bill is solely decided by user him/herself.
- Group Game: 
This type of game deals with the shared energy bill, such like AC, heating, ventilation, lighting, etc. The occupancy of the shared room should be monitored so as to map the energy bill to all the occupants in the space. Due to different comfort level and personal preference for temperature and lighting condition, the reward from host to the group users might not be evenly distributed users in the space. The game need to develop a mechanism that stimulate the collaborations amongst the users to reach a consensus on the temperature setup and lighting scheme that reduce the overall energy cost.
The following picture shows our system as well as the deployment situation. The backbone of the entire system is the local area network. It serves as a basis for different devices to communicate with different protocols. Four subsystems are connected to the LAN, that is, the lighting subsystem, the air conditioning subsystem, the sensing subsystem and the smart meter subsystem. The smart meter subsystem focuses on individual behavior monitoring. . It’s a wireless smart meter network that collects real-time energy consumption information and sends the data back to our server.

### Testbeds
![Rohm](../../../images/blog/soc-rohm.jpg) ![Cory](../../../images/blog/soc-cory.jpg)