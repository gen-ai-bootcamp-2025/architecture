# architecture
architecture

## functional requirement

The company want to extract the sub_skills by theme skills of a resume by semantic analysis and compare to position. 
The goal is to understand the is the resume fir the position on the skills approach.
The theme skills are defined by the user accross the interface for the defaut sub-skills.
Also in function of the resume the user can define accross interface new theme subskills.
the number subskills must be 5 by theme skills.

The result  must be displyed in function of the language interface. If the default language is French but the user want the result in english, the information must be displayed in english with a french user interface.

The information must be displayed like this :

- The theme of the subskills
- the subskills
- the evaluation of the subskills in function the cv compare to the position
- the note explanation of the subskills choice

## assumptions

The enginneer decided to use chatGPT to extract and analyse the information. the user can only use create the default sub skills theme and create for each cv a new shub skills theme if needed.

## Data strategy
- the resume and the position are uploaded in pdf or word
- To optimize the vector the data must be cleaned 
- The data is sent and the result must be in json

## Risk
The user does not have access to the prompt, no risk
The risk is only if the data is not a resume or a position

## Model Selection and Development
The business model choosen :
    - Cloud approach for the website
    - Input-Output: text-to-text?
    - Number of models needed : 1
    - Fine-tuning requirements : No could manage by a prompt
    - Model performance and efficiency : The response must be under less 1 second ig the user create an action

## Integration and Deployment
    - Github for the development
    - Deployment on a cloud hosting

## Monitoring and Optimization
    - All information is saved inside the database
    - All token and price is saved inside the database
    - All the response time is saved inside the database
    - The feedback will be by the user about the result quality

## Governance and Security
    - All the data about the resume is saved in AES 256
    - the encryption and the decryption is just to send the information to the llm

## Scalability and Future-Proofing
    - If needed the server  can be improved because  we take a cloud approach
    - The prompt will be optimize easily. If the result is not correct, a fine tuning approach can be done.

    

    



    
    
