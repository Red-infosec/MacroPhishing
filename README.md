# MacroPhishing
Word resources for phishing. Includes "Click Enable Content" bait and decoy document deployment. I was inspired by Cerber ransomware documents when I designed the bait. 

To use, open template.doc and create new macros. For the main module, paste in the code from main.vba. Then create a new Class Module named "oAppClass" or rename it to whatever, but make sure the name matches that in the main module. Paste in the code from oAppClass.vba. Add in your code to run your malware. For the decoy, put in your decoy text in the "Decoy goes here in hidden text." section. Then, select all of the decoy text, and set the font to hidden. This hides it from the user when the macro is not executed. When the macro runs, it deletes the first page (the bait), and unhides all text (displays the lure). Then, it automatically chooses not to save the changes, so that the user does not get the "would you like to save" prompt, and the macro doesn't delete the decoy after future views. 

