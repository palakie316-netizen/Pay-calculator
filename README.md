# Pay Planner (Web App / PWA) v4

v4 changes:
- Travel is treated as "separate":
  - Travel hours are paid at base rate
  - Travel hours do NOT count toward overtime threshold
  - OT premium applies ONLY to OT WORK hours
- Weekly OT threshold applies to WORK hours only
- Everything else remains: mobile calendar, 12h + manual, VA/pension, 2-week pay period

Formulas:
- Base pay = rate * (work_hours + travel_hours)
- OT premium = (mult - 1) * rate * (OT_work_hours)
