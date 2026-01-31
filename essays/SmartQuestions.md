---
layout: essay
type: essay
title: "Questionable Queries get Quibble and Answers from Quacks"
# All dates must be YYYY-MM-DD format!
date: 2025-01-29
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

What is a smart question? What is a dumb question? Some say that there are no “dumb” questions, but in the software engineering space, there are definitely questions that have room for improvement according to “How To Ask Questions The Smart Way” by Eric Steven Raymond. 

Before artificial intelligence had the ability to answer questions with a reasonable amount of sense, many turned to spaces like Google and StackOverflow in order to have their inquiries answered. Here, experts in their respective fields would provide replies to a posted question in an attempt to help the poster. This is where asking “smart” questions came to be of significance. 

A “smart” question is clear, concise, thoughtful, polite, grammatically correct, and shows effort. In “How To Ask Questions The Smart Way” Raymond details how to ask questions to hackers specifically. This is different from querying a “normal” person. Because it is technical problems that are being asked, it must fulfill certain requirements. A good example of a “smart” question is below. Let's examine what makes this question so good, and how they received an answer to their question within 2 days. 


```
Q: How to filter DataRow using % character

I wish to filter DataRow values using a condition like this:

dr.RowFilter = "CODE LIKE '%01%2%'"

This raises an error:

System.Data.EvaluationException: string pattern is not valid

I tried to embrace the wildcard character between square brackets (ie: %01[%]2%). It works, but returns an empty result set.

How can I use the special character between my filter string?

```
You can learn more at [StackOverflow: How to filter DataRow using % character]([https://keigo-zoo.lovable.app](https://stackoverflow.com/questions/79878096/how-to-filter-datarow-using-character)).

This user was very clear about their goal from the start. They provided an example and went on to concisely explain the problem that they were having. They cited what they have already tried, and what the results of that were. Then, they politely posed a question. Everything was grammatically correct, and did not involve any superfluous language. In the following thread, others replied to this question. Although not all of them answered the question, the poster was polite and remained steadfast in their manners and effort to solve the problem. Eventually someone posted an answer. The original question had an upvote on it, demonstrating that this may have been a question that was also valuable to another person. 

## Dumb questions deserve “smart” answers

Below is an example of a question that could be worded a little better. 

```
Q: react native keyboardAwareScrollView

<KeyboardAwareScrollView
  style={{ flex: 1 }}
  behavior={Platform.OS === 'ios' ? 'padding' : 'height'}
  contentContainerStyle={{ flexGrow: 1}}
  enableOnAndroid={true}
  extraScrollHeight={getPlatForm() === 'android' ? 80 : 0}
  enableAutomaticScroll={getPlatForm() === 'android'}
  keyboardShouldPersistTaps="handled"
  showsVerticalScrollIndicator={false}
  keyboardOpeningTime={Platform.OS === 'ios' ? 0 : 250}
>
  <View style={pageStyles.inputMinusSpace}>
                <TextInput
                  label="Note"
                  multiline
                  mode="flat"
                  style={[pageStyles.input,Styles.DefaultInput,pageStyles.customInput, { height: 80, textAlignVertical: 'top' }]}
                  underlineColor={ColorsApp.BorderColor}
                  activeUnderlineColor={ColorsApp.PRIMARY}
                  textColor={ColorsApp.textColor}
                  contentStyle={{ backgroundColor: 'transparent' }}
                  value={managerNote}
                  onChangeText={setManagerNote}
                  scrollEnabled={false}
                />
              </View>
</KeyboardAwareScrollView>

i am use like this...when i focus on textinput...only half textinput is visible because this is multiline...

i try to multiple option like extraHeight and others...anyone help me

```
You can learn more at [StackOverflow: react native keyboardAwareScrollView]([https://keigo-zoo.lovable.app](https://stackoverflow.com/questions/79879881/react-native-keyboardawarescrollview)).

The poster started by putting a chunk of code at the start of their post that was titled with lowercase letters. After they provided the code that they needed help with, they put two lines of text that described one alternative that they tried. This is not very helpful to a user who would want to potentially help this poster. They also did not have proper grammar or spacing. Although English may not be their first language, it would be helpful if they mention this in their post if this is the case. They end with a plea for help, which generally does not do much to elicit urgent responses from hackers. This question has not received any answers or replies yet. 
 

## Conclusion

As a result of this experience, I have learned what the “culture” of StackOverflow was like. I was amazed by the network of resources and people's willingness to answer questions for free. I believe that “How To Ask Questions The Smart Way” was a good read for anyone who is interested in posing a question in a similar space. I think that this was a good resource for even those who do not post to these types of forums, because it is similar to prompt engineering. The better the question is curated, the more artificial intelligence can help you. Artificial intelligence is on the rise, and provides instant answers to users. This may be why it has been growing in popularity, reducing the number of questions that are being posted to different threads and forums. 
