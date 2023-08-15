#perspective_nlzr 

This folder contains the information that is required to set up a fully configurable multi-perspective analyzer prompt via chatGPT (and possibly others).

Several approaches have been tested, of which three are provided here:  

1. Prompt only multi-perspective analyzer; for copy-pasting directly into message, or to edit and incorporate in larger prompts (for example see [2]).  
2. XGREPLIST multi-perspective analyzer; pre-configured to accept Data_ID's, doc_id's, customized text/variables/input/etc.; also allows for extracting perspectives from Data_ID's, doc_id's, customized text/variables/input/etc., after which extracted perspectives can be used on other Data_ID's, doc_id's, customized text/variables/input/etc.  
3. Stand-alone fully configurable multi-perspective analyzer; allows for configuration of all options; see extended readme_nlzr.  


#Basic practical example:

Upload your CV and use the related doc_id to have CV reviewed by any perspectives of choice:

Your_CV doc_id = 123456789

run `eyes 123456789 (Perspective_1) (Perspective_2) (Perspective_3) (Perspective_4)`

Result: [img]



#Advanced practical example:

XGREPLIST √