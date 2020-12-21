## Proposed

Pipeline manager to chain independent processes into single pipeline.

#### Pipeline 

Scheduled task which will trigger all processes in that pipeline into await status. Independant tasks will be fired immediatelly or by their own delay. 

Pipeline has it's own dispatcher process which will schedule all pipeline processes into one pipeline execution process.

#### Proccess 

Process is a part of pipeline which can has it's own delay, can be dependent of other processes and has it's own execution timeout. 

Every process has few statuses:
- Await 
- Execution
- Success
- Failed
