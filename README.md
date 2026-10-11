# Corner-l
services:   - type: web     name: corner-lab     runtime: node     plan: free     buildCommand: npm install     startCommand: npm start     healthCheckPath: /api/status     envVars:       - key: API_FOOTBALL_KEY         sync: false       - key: MATCH_WINDOW         value: "10"       - key: DAILY_API_BUDGET         value: "90"
