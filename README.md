# Genetic Algorithm for Knapsack Problem
AI Course Exercise

## **<ins>Algorithm Details</ins>**:

### **Representation:** 
binary
### **Population Init:** 
random
#### **Population Size:**
2 * chromosome length
### **Recombination:** 
k-point cross over (I generate every possible child: 2^(k+1)-2 children)
### **Mutation:** 
bit-flip (with a probability of 0.02 for each gene)
### **Fitness Function:**
values sum - penalty
(I change negative fitnesses to a small positive number to give them a chance)
### **Parent Selection:**
proportional select
### **Offspring Generation:**
[3 * population size] new children
### **Survival Selection:**
proportional select (among offspring)
### **Termination Condition:**
when for k=100 generations, changes of the best fitness among population is less than epsilon=%5 OR we reach the 200th generation
