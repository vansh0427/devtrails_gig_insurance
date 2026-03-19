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
