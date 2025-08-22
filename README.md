--
# supply_chain_optimization_models
--
REPOSITORY CONTAINING OPTIMIZATION MODELS SUCH AS LP, IP AND MIP MODELED UTILING PuLP fron Python

### WHAT IS A SUPPLY CHAIN ?

A supply chain consists of all parties involved in the process of fulfilling a customer request.

- Includes
    - suppliers
    - Internal Manufacturers
    - 3PLS

### WHAT IS SUPPLY CHAIN OPTIMIZATION? 
Optimizations aims for the most effective process of fulfilling a customer request given existing constrains. 

<img width="1958" height="716" alt="image" src="https://github.com/user-attachments/assets/c7b255ac-7d5c-4a11-b5b9-728fe1ffa4fd" />


* Contrains could include but are not limited to:
    * cost 
    * space utilization 
    * time
 
---
### BUILDING A MODEL AND LINEAR PROGRAMMING
---

AN OVERVIEW INTO LINEAR PROGRAMMING 

- Refers to modeling and solving a problem mathematically.

When both **objective function** and the **constrain →** are linear, the problem is referred as linear programming. 

Linear functions ⇒ each variable appears as a separate term raised to the first power and is multiplied by a constant [can be 0]

**Common LP Applications** 

- Two or more products produced using limited resources
- Maximize profit based on the profit contribution per unit of each product
- Determine how many units of each product to produce

AN OVERVIEW ON OPTIMIZATION MODELS 

Optimization Models Include:

- **Objective function**
    - mathematical expression that describes the problem.
- **Constrains**
    - Limitations
- **Uncontrollable inputs**
    - Not under the control of decision maker.
- **Decision Variable**
    - Controllable inputs

AN OVERVIEW OF INTEGER PROGRAMMING 
One of the assumptions of linear programming is that decision variables can take on fractional values.

> Integer programming ⇒ use of special variables that must be within 0 - 1
>

- ***Three types of problems***
    - **Pure**
        - all variables are integer
    - **Mixed**
        - some but not all variables have integer values
    - **Zero-one**
        - special case where decision variable's must have solution values 0 → 1

There are situations in which only some of the variables are restricted to integers.  Mixed-integer programming (MIP) problem

One common use of 0-1 variables involves limiting the number of projects or items that are selected from a group.


### PYTHON PULP

PuLP is a python library written specially to write IP and LP models. It interacts with different solvers such as

- [GLPK](http://www.gnu.org/software/glpk/glpk.html)
    - GNU Linear Programming Kit
- COIN-OR  CLP/[CBC](https://github.com/coin-or/Cbc)
- [CPLEX](http://www.cplex.com/)
    - IBM® ILOG® CPLEX® Optimization Studio is a prescriptive analytics solution that enables rapid development and deployment of decision optimization models using mathematical and constraint programming.
- [GUROBI](http://www.gurobi.com/)
and others....



Here's a python repo with several examples https://github.com/coin-or/pulp/tree/master/examples
