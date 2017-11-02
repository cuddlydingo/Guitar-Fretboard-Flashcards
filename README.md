#       v1.0, 2016.09.24
#       Author: Brodie Phillips

#       ===============================================================================
#       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#       ===============================================================================

#       READ ME!!!
#       You can change the strings which are being quizzed by (un)commenting out the
#       various dictionary entries.  It might be easier to start out by only studying
#       a few strings at a time.

#       ===============================================================================
#       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#       ===============================================================================


import random


#       Dictionary values
q_dictionary = {
        "What is the 6th string open?" : "E",
        "What is the 6th string 1st fret?" : "F",
        "What is the 6th string 2nd fret?" : "F#",
        "What is the 6th string 3rd fret?" : "G",
        "What is the 6th string 4th fret?" : "G#",
        "What is the 6th string 5th fret?" : "A",
        "What is the 6th string 6th fret?" : "A#",
        "What is the 6th string 7th fret?" : "B",
        "What is the 6th string 8th fret?" : "C",
        "What is the 6th string 9th fret?" : "C#",
        "What is the 6th string 10th fret?" : "D",
        "What is the 6th string 11th fret?" : "D#",
        "What is the 6th string 12th fret?" : "E",

        "What is the 5th string open?" : "A",
        "What is the 5th string 1st fret?" : "A#",
        "What is the 5th string 2nd fret?" : "B",
        "What is the 5th string 3rd fret?" : "C",
        "What is the 5th string 4th fret?" : "C#",
        "What is the 5th string 5th fret?" : "D",
        "What is the 5th string 6th fret?" : "D#",
        "What is the 5th string 7th fret?" : "E",
        "What is the 5th string 8th fret?" : "F",
        "What is the 5th string 9th fret?" : "F#",
        "What is the 5th string 10th fret?" : "G",
        "What is the 5th string 11th fret?" : "G#",
        "What is the 5th string 12th fret?" : "A",

#       "What is the 4th string open?" : "D",
#       "What is the 4th string 1st fret?" : "D#",
#       "What is the 4th string 2nd fret?" : "E",
#       "What is the 4th string 3rd fret?" : "F",
#       "What is the 4th string 4th fret?" : "F#",
#       "What is the 4th string 5th fret?" : "G",
#       "What is the 4th string 6th fret?" : "G#",
#       "What is the 4th string 7th fret?" : "A",
#       "What is the 4th string 8th fret?" : "A#",
#       "What is the 4th string 9th fret?" : "B",
#       "What is the 4th string 10th fret?" : "C",
#       "What is the 4th string 11th fret?" : "C#",
#       "What is the 4th string 12th fret?" : "D",

#       "What is the 3rd string open?" : "G",
#       "What is the 3rd string 1st fret?" : "G#",
#       "What is the 3rd string 2nd fret?" : "A",
#       "What is the 3rd string 3rd fret?" : "A#",
#       "What is the 3rd string 4th fret?" : "B",
#       "What is the 3rd string 5th fret?" : "C",
#       "What is the 3rd string 6th fret?" : "C#",
#       "What is the 3rd string 7th fret?" : "D",
#       "What is the 3rd string 8th fret?" : "D#",
#       "What is the 3rd string 9th fret?" : "E",
#       "What is the 3rd string 10th fret?" : "F",
#       "What is the 3rd string 11th fret?" : "F#",
#       "What is the 3rd string 12th fret?" : "G",

#       "What is the 2nd string open?" : "B",
#       "What is the 2nd string 1st fret?" : "C",
#       "What is the 2nd string 2nd fret?" : "C#",
#       "What is the 2nd string 3rd fret?" : "D",
#       "What is the 2nd string 4th fret?" : "D#",
#       "What is the 2nd string 5th fret?" : "E",
#       "What is the 2nd string 6th fret?" : "F",
#       "What is the 2nd string 7th fret?" : "F#",
#       "What is the 2nd string 8th fret?" : "G",
#       "What is the 2nd string 9th fret?" : "G#",
#       "What is the 2nd string 10th fret?" : "A",
#       "What is the 2nd string 11th fret?" : "A#",
#       "What is the 2nd string 12th fret?" : "B",

#       "What is the 1st string open?" : "E",
#       "What is the 1st string 1st fret?" : "F",
#       "What is the 1st string 2nd fret?" : "F#",
#       "What is the 1st string 3rd fret?" : "G",
#       "What is the 1st string 4th fret?" : "G#",
#       "What is the 1st string 5th fret?" : "A",
#       "What is the 1st string 6th fret?" : "A#",
#       "What is the 1st string 7th fret?" : "B",
#       "What is the 1st string 8th fret?" : "C",
#       "What is the 1st string 9th fret?" : "C#",
#       "What is the 1st string 10th fret?" : "D",
#       "What is the 1st string 11th fret?" : "D#",
#       "What is the 1st string 12th fret?" : "E"
}




# Scoring Trackers
correct_answers = 0
wrong_answers = 0


# Start asking questions:
for i in q_dictionary:
        if input(str(i + " ")) == q_dictionary[i]:
                correct_answers += 1
                print("Correct!")
        else:
                wrong_answers += 1
                print("Sorry, practice harder")


# Calculate Score
total_answers = correct_answers + wrong_answers
final_score_1 = (correct_answers / total_answers) * 100
final_score_2 = format(final_score_1, '.2f')

print("\n")
print("Your final score was " + str(final_score_2) + "%")


# End of file.
 
