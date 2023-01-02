class Solution(object):
    def isValid(self, s):
        """
        :type s: str
        :rtype: bool
        """
        # Stack for left symbols
        stack = []
        # Loop for each character of the string
        for c in s:
            # If left symbol is encountered
            if c in ['(', '{', '[']:
                stack.append(c)
            # If right symbol is encountered
            elif c == ')' and len(stack) != 0 and stack[-1] == '(':
                stack.pop()
            elif c == '}' and len(stack) != 0 and stack[-1] == '{':
                stack.pop()
            elif c == ']' and len(stack) != 0 and stack[-1] == '[':
                stack.pop()
            # If none of the valid symbols is encountered
            else:
                return False
        return stack == []
