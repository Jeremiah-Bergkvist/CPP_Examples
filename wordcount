#include <iostream>
#include <string>

int main()
{
   std::string s1 = " This is a test		string.";
   size_t word_start = 0;
   size_t word_len = 0;
   unsigned int word_count = 0;
   
   for(size_t index = 0; index < s1.size(); index += 1)
   {
       if(s1[index] == ' ' || s1[index] == '\t')
       {
           // Could extract the word and add it to an array.
           if(word_len > 0)
           {
               word_count += 1;
               std::cout << word_count << ": " <<  s1.substr(word_start, word_len) << std::endl;
               
           }
           word_start = index + 1;
           word_len = 0;
           continue;
       }
       else
       {
           word_len += 1;
       }
   }
   // Could extract the word and add it to an array.
   if(word_len > 0)
   {
       word_count += 1;
       std::cout << word_count << ": " <<  s1.substr(word_start, word_len) << std::endl;
   }
   return 0;
}
