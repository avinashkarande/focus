# focus

def solution(input_string):
    output_string = ''
    digit = int(input_string[1])
    
    digit_count =0
    for  char in input_string:
        if char.isdigit():
            digit_count +=1
            
    if digit == len(input_string):
        output_string = 'A'
    elif input_string.count('a') ==2:
        output_string = 'B'
    elif 'infosys' in input_string:
        output_string = 'C'
    elif digit_count ==1:
        output_string ='D'
        
    return output_string

print(solution('r7akes1'))
print(solution('24activate'))
print(solution('42infosysmysore'))
print(solution('a2ctive'))
