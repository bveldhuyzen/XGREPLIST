#perspective_nlzr 

This folder contains the information that is required to set up a fully configurable multi-perspective analyzer prompt via chatGPT (and possibly others).

Several approaches have been tested, of which three are provided here:  

1. Prompt only multi-perspective analyzer; for copy-pasting directly into message, or to edit and incorporate in larger prompts (for example see [2]).  
2. XGREPLIST multi-perspective analyzer; pre-configured to accept Data_ID's, doc_id's, customized text/variables/input/etc.; also allows for extracting perspectives from Data_ID's, doc_id's, customized text/variables/input/etc., after which extracted perspectives can be used on other Data_ID's, doc_id's, customized text/variables/input/etc.  
3. Stand-alone fully configurable multi-perspective analyzer; allows for configuration of all options; see extended readme_nlzr.  
  
____


#Basic practical example:

Upload your CV and use the related doc_id to have CV reviewed by any perspectives of choice:

>Full Job description:  
>
>Looking for competent complaint manager at $COMPANY's department for handling escalations/complaints not of judicial nature. Involves much paperwork and typing/email to address customer concerns and complaints. Requires empathy, problem-solving skills, and ability to address customer complaints within SLA. $COMPANY is a manufacturer of electrical heating devices of medium quality for household purposes. Complaints are mostly about defective devices due to improper use by user. Low percentage of complaints involves defective device due to manufacturing error, or to defective device due to improper shipping. On very rare occasion complaint is received of judicial nature; complaint manager is to recognize these and submit to legal department.  
>  
> List of requirements here  
> List of preferences here  
> etc.  

Your_CV doc_id = 123456789

>`eyes 123456789 (Simple-minded HR employee that specializes in acquiring new employees via LinkedIn. Uses LinkedIn primarily to review initial responses to job openings; pays less attention to meaning of content, truth of content, CV; pays more attention to presentation. If unsure, then tends to specifically select applicants on use of the right key words, which are: soft skills, empathy, team player, inclusion/inclusive, equality) (Manager of HR department that makes the final decision on whether or not applicant is suitable and will be offered the job. Reads CV thoroughly; pays great attention to related job experience and interests, and asks probing questions to confirm experience level. Rejects applications if finding mistakes in spelling, grammar, use of interpunction, use of capitals. Great preference for well-versed applicants with proven track-record at more than one employer) (Employee of HR department on a Monday after a long weekend of partying and drinking; does not really want to read much and spend time on investigating applicants with extensive CV. Prefers easy to read and easy to understand CV's. Might reject because of anything that might perceived as unclear or underqualified or overqualified) (Hardcore veteran of HR department that reads all documentation provided by applicant. Respects honesty and those looking for challenges. Adheres usually to strictly that which is requested, but on occasion can make exceptions for underdog applications to investigate if maybe a wizard in the making is applying.)`

Result: [img]



#Advanced practical example:

XGREPLIST √