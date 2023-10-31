tags:: Software Development
topic:: [[Problem-solving Approach]]
softdev:: Unit 3 Outcome 1

-
- ```mermaid
  
  flowchart TD
      A[Problem-solving methodology]:::main --- B[Analysis]:::stage
      A --- C[Design]:::stage
      A --- D[Development]:::stage
      A --- E[Evaluation]:::stage
      B -- Activities --- B1[Solution requirements]:::activity
      B1 ---  B2[Solution Consraints]:::activity
      B2 ---  B3[Solution Scope]:::activity
      C --Activities --- C1[Solution Design]:::activity
      C1 ---  C2[Evaluation Criteria]:::activity
      D -- Activities --- D1[Manipulation]:::activity
      D1 --- D2[Validation]:::activity
      D2 --- D3[Testing]:::activity
      D3 --- D4[Documentation]:::activity
      E -- Activities ---E1[Solution Evaluation]:::activity
      E1 --- E2[Evaluation Strategy]:::activity
  classDef activity fill:#eee,stroke:black
  classDef main stroke-width:3,fill:white,stroke:black
  classDef stage stroke-width:2,stroke:black
  ```
  *If you can't see the Mermaid diagram above, install the Fenced Code Plus plugin*
-
- comprised of the four stages
	- [[Analysis Stage]]
	- [[Design Stage]]
	- [[Development Stage]]
	- [[Evaluation Stage]]
- each stage has a set of activities as shown in the diagram above
- if using the [[Waterfall Model]], the stages are completed once, in order
- if using the [[Agile Model]] or the [[Spiral Model]], the four stages are completed in order for each iteration of the model