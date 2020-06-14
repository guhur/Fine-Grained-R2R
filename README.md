# Fine-Grained R2R
Code and data of the Fine-Grained-R2R Dataset proposed in paper Sub-Instruction Aware Vision-and-Language Navigation

* The code and data are pre-released and confidential to close collaborators/colleagues only, the copyright resides with the authors of the paper Sub-Instruction Aware Vision-and-Language Navigation, please do not distribute.
* This dataset is build upon the [Room-to-Room (R2R) dataset](https://github.com/peteanderson80/Matterport3DSimulator/tree/master/tasks/R2R), we refer the readers to its repository for more details.

## data
The Fine-Grained R2R data, which enriches the R2R dataset with sub-instructions and their corresponding paths. The overall instruction and trajectory of each sample remains the same.

* For paths in the train, the validation seen and the validation unseen splits, we add two new entries:
  * **new_instructions**: A list of sub-instructions produced by the **Chunking Function** from the original instructions.
  * **chunk_view**: A list of sub-paths corresponding to the sub-instructions, where each number in the list is the index of a viewpoint in the ground-truth path. The index starts at 1.
  
* Some sub-instructions which refer to camera rotation or a *STOP* action could match to a single viewpoint.

* For the test unseen split, we only provide the sub-instructions but not the sub-paths.


## source
