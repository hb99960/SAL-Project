# Assignment S13

---

### **1. When should you prioritize *latency* over *throughput* in a distributed system?**

A) When processing batch analytics on logs
B) When building a real-time multiplayer game
C) When generating monthly reports
D) When storing large volumes of data

**Answer:** B

---

### **2. What’s the main tradeoff of using vertical scaling over horizontal scaling?**

A) More fault tolerance
B) Easier to distribute requests
C) Hardware limitations and no failover
D) Cheaper infrastructure cost

**Answer:** C

---

### **3. Why does *normal hashing* fail in distributed systems when scaling out servers?**

A) Because it uses random numbers
B) Because it always maps to a new IP address
C) Because most keys are remapped, causing cache misses
D) Because it doesn’t support parallel processing

**Answer:** C

---

### **4. A system needs to process 50,000 requests/sec with < 100ms response time. What is the most suitable design tradeoff?**

A) Favor strong consistency over availability
B) Prioritize throughput and use eventual consistency
C) Scale vertically to simplify architecture
D) Use a stateful server for fast response

**Answer:** B

---

### **5. Which of the following systems is more likely to benefit from *stateless* server design?**

A) Online Chess Match
B) Live Stock Trading
C) E-commerce Home Page
D) Chat Support Application

**Answer:** C

---

### **6. Which technique is best for preventing a service from being overwhelmed by too many requests in a short period?**

A) Consistent Hashing
B) Rate Limiting
C) Load Balancer
D) Horizontal Scaling

**Answer:** B

---

### **7. In a distributed system, which combination best reflects LinkedIn's strategy to reduce page load time by 60%?**

A) Vertical scaling + eventual consistency
B) Load balancing + consistent hashing
C) Caching + reducing backend round-trips
D) Stateless servers + batch processing

**Answer:** C

---

### **8. Which tradeoff does a system make when choosing *stateful servers* over stateless ones?**

A) Higher fault tolerance
B) Simplified request routing
C) Difficulty in scaling and session replication
D) Increased horizontal scalability

**Answer:** C

---

### **9. If your system is experiencing low latency but very poor throughput, what is a likely cause?**

A) All services are stateful
B) Each request is processed in parallel
C) The system uses micro-batching
D) Requests are not being queued properly or pipelined

**Answer:** D

---

### **10. In consistent hashing, adding a new server impacts:**

A) All existing mappings
B) Only a fixed small number of keys
C) Only the largest partitions
D) Nothing, as hashing stays unchanged

**Answer:** B

---

## **Descriptive Questions**

---

### **1. In a real-world application like Instagram or LinkedIn feed, explain how caching improves latency. What are the tradeoffs of over-caching?**

- You can mention how cache reduces trips to backend/DB.
- But also the risk of stale data and cache invalidation complexity.

---

### **2. Explain how you would design a URL shortener like Bitly. What components would you use and how would you ensure it scales?**

- Expect answers involving database, hashing, service layers, possible use of cache, rate limiting, and load balancer.

---

### **3. Describe a scenario where choosing availability over consistency is the right tradeoff. How does this decision affect the user experience?**

- Use cases: social media, metrics collection, newsfeed.

---

### **4. Why might a company like Netflix prefer high throughput in their order or stream processing pipeline, even if latency is slightly higher?**

- Highlight how bulk processing of recommendations or stream logs is more valuable than real-time feedback.

---

### **5. In load balancing, compare round-robin vs consistent hashing in terms of scaling and user session consistency. Which would you use in a video streaming app and why?**

- Show understanding of stateful user experience (e.g., playback sessions) and how consistent hashing supports sticky sessions.