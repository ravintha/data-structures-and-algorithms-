
#######################
## An anagram is when the two strings can be written using the exact same letters
## For example:

### "public relations" is an anagram of "crap built on lies."

###"clint eastwood" is an anagram of "old west action"

##easy implemetation###
def anagram(s1,s2):
    
    # Remove spaces and lowercase letters
    s1 = s1.replace(' ','').lower()
    s2 = s2.replace(' ','').lower()
    
    # Return boolean for sorted match.
    return sorted(s1) == sorted(s2)

#######################
#Manual implemetation#
######################


def anagram(a1,a2):
    
    # Remove spaces and lowercase letters
    a1 = a1.replace(' ','').lower()
    a2 = a2.replace(' ','').lower()
    
    # Edge Case to check if same number of letters
    if len(a1) != len(a2):
        return False
    
    # Create counting dictionary (Note: could also use DefaultDict from Collections module)
    count = {}
    
       
    # Fill dictionary for first string (add counts)
    for letter in a1:
        if letter in count:
            count[letter] += 1
        else:
            count[letter] = 1
            
    # Fill dictionary for second string (subtract counts)
    for letter in a2:
        if letter in count:
            count[letter] -= 1
        else:
            count[letter] = 1
    
    # Check that all counts are 0
    for c in count:
        if count[c] != 0:
            return False

    # Otherwise they're anagrams
    return True
    
###############
# to run
anagram('dog','god')
anagram('clint eastwood','old west action')
anagram('aa','bb')
