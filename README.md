# Week 2: Front-End Application Development

Contains the source code for the front-end interface built with React.

## Instructions
Run `npm install` followed by `npm start` to run locally.
class Solution {
public:
    int strStr(string haystack, string needle) {
        if (needle.empty()) {
            return 0;
        }

        int haystackLength = haystack.length();
        int needleLength = needle.length();

        if (needleLength > haystackLength) {
            return -1;
        }

        for (int startIndex = 0; startIndex <= haystackLength - needleLength; startIndex++) {
            if (haystack.substr(startIndex, needleLength) == needle) {
                return startIndex;
            }
        }

        return -1;
    }
};
