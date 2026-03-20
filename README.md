# DevTrails Gig Insurance  
AI-driven platform protecting gig workers from income loss due to real-world disruptions.
##  Persona & Requirement

We are targeting **gig workers**, specifically Q-commerce delivery partners such as **Blinkit**.

These workers typically earn around **₹500–₹1000 per day** and rely entirely on completing deliveries for their income. Their earnings are highly unstable and directly affected by external factors such as weather conditions, pollution, and other real-world disruptions.

Example :
During heavy rainfall, delivery demand drops significantly, leading to a **30–40% reduction in daily income**, and in extreme cases, even a **100% loss of income** for that period.

Currently, there is **no existing solution** that provides financial protection for gig workers against such income loss caused by external disruptions.

Our goal is to design a system that provides **income protection for gig workers during such events**.

## Workflow

1. The user registers on the platform by providing details such as location,working hours, and their delivery platform.
2. The system analyzes external data such as AQI Levels, Weather Condition and other data to calculate user's risk profile.
3. Based on risk , weekly premium plan is generated dynamically .
4. User subscribes to weekly insurance policy.
5. System continuously monitors real -time data through API.
6. When parametric trigger is detected , system automatically identifies potential income loss
7. Payout is automatically initiated wihout requiring any claim from user

## Weekly premium model
Our platform uses a **dynamic weekly premium model** that is easy for gig workers to understand and afford.

Instead of a fixed price for everyone , the premium depends on how risky the worker's environment is. It Works like the workers who are in **safer areas** pays a **lower** premium and the one who are in **riskier areas** pays a slightly **higher** premium.

### Basic Motto:
Workers pay a small weekly amount, and in return, they are protected from sudden income loss caused by real-world disruptions.

## Parametric Triggers
Payouts are not manual, they are triggered automatically based on real-world conditions.
If any of the conditions like rainfall , local disruptions cross a predefined limit , the system assumes that the worker's income will affected and triggers instant payout.

## Payout is "event" based not "time based"
Worker receives payout only when :
-> Disruption occurs
-> Worker is active
-> Policy is also active

If no disruption happens , no payout is made.

##  Platform Choice 

We will use a mobile approach , as delivery partners are usually active on mobile.
Mobile app allows:
--> Real time updates
--> Better Location Tracking

##   AI & Fraud Detection

### AI Usage:
- Predicts risks on the basis of weather and location
- Dynamically adjustment of weekly premium model

### Fraud Handling:
- Cross Checked GPS data.
- Unusual claims like worker is just registered only but did not work
- Multiple claims from same area sudden

## Tech Stack
- Frontend :  React
- Backend  :  Node.js
- Database :  MongoDB
- AI/ML    :  Python(Scikit Learn)
- Payments :  Razorpay
  
