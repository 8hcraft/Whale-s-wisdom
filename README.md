# Whale-s-wisdom

### **Aavegotchi Mentor Points System**  
*(A Win-Win for Whales, Newbies & the DAO)*  

---

#### **1. What Are Mentor Points?**  
- **Non-tradable tokens** earned by experienced players (whales) for:  
  - Teaching newbies poker strategy  
  - Sponsoring weak Gotchis in games  
  - Creating beginner-friendly content (guides, memes)  
- **Redeemable** for exclusive rewards (see Section 3).  

---

#### **2. How to Earn Mentor Points**  
| **Action**                     | **Points Earned** | **Example**                                  |  
|--------------------------------|------------------|---------------------------------------------|  
| Play 10 hands with a newbie    | +5               | Whale + newbie duo at Pity Poker tables     |  
| Win a game with a weak Gotchi  | +3               | Whale carries a 50-trait Gotchi to victory  |  
| Write a strategy guide         | +10              | "How to Read Tells in Gotchi Poker" post    |  
| Create a tutorial video        | +15              | YouTube walkthrough of trait optimization   |  

**Smart Contract Snippet (Tracking Points)**:  
```solidity  
function awardMentorPoints(address mentor, uint256 points) external {  
    require(isApprovedMentor[mentor], "Not a verified mentor");  
    mentorPoints[mentor] += points;  
    emit PointsAwarded(mentor, points);  
}  
```  

---

#### **3. Redeeming Mentor Points**  
| **Reward**                     | **Cost**  | **Purpose**                                 |  
|--------------------------------|----------|--------------------------------------------|  
| "Mentor" Wearable (NFT)       | 20 pts   | Flex status in-game                        |  
| Custom Gotchi Title (e.g., "Professor") | 50 pts | Social cred                   |  
| DAO Governance Voting Power   | 100 pts  | Influence future updates                   |  
Etc. TBD by Aavegotchi DAO whales.

---

#### **4. Anti-Abuse Safeguards**  
- **Newbie Feedback**: Recipients rate mentors (1-5 stars).  
  - Low-rated mentors earn **half points** for 1 week.  
- **Cooldowns**: Max 10 points/day from playing with the same newbie.  
- **DAO Oversight**: Council can ban exploiters.  

---

#### **5. Why Whales Will Love This**  
- **Status Symbols**: Exclusive wearables/titles show seniority.  
- **Real Influence**: Governance power over game updates.  
- **Community Clout**: Featured in "Top Mentors" leaderboards.  

---

#### **6. DAO Benefits**  
- **Retains Whales**: Gives them purpose beyond farming.  
- **Boosts Retention**: Newbies stay longer with guidance.  
- **Free Content**: Guides/videos market the game organically.  

**Example Workflow**:  
1. Whale **@Alice** teaches **@Bob** how to bluff.  
2. Alice earns **5 Mentor Points**.  
3. Alice redeems points for a **"Poker Pro" title**.  
4. Bob sticks around, buys wearables → **DAO profits**.  
