# Assignment_1B


<h1><center><font size="40"><u>1)CHANNELS</u></center></font></center></h1>

1. A convolutional layer takes a certain number of input channels (I) and calculates a specific number of output channels (O).

2. Channels gives us an idea about the location and size of the image.
3. It gives us information about a specific feature.
4. Channels as taught to us are only RGB but complex channels also do exist.
![](https://cdn-images-1.medium.com/max/1600/1*FBvMDT1DEfJvcNpSkf86VQ.png)

![](https://i.stack.imgur.com/kczF0.png)

<h1><center><font size="40"><u>2)KERNELS</u></center></font></center></h1>

1. Kernel is a type of operator that operates on the entirety of the image such that it encodes and gives out what information the pixels     have embedded within them.

2. It forms an important and integral component of the layered structure.
3. It generally is represented in the form of a matrix.
4. An image kernel is a small matrix used to apply effects like the ones you might find in Photoshop or Gimp, such as blurring, sharpening     of edges etc.
5. They're also used in machine learning for 'feature extraction'.

![](https://mlnotebook.github.io/img/CNN/convSobel.gif)

# The reasons why 3*3 kernel is better?
Stacking smaller convolutional layers is lighter, than having bigger ones. It also tends to improve the result, with the simple intuition that it results in more layers and deeper networks.
![](https://cdn-images-1.medium.com/max/1400/1*nrrxmXzOJo_XHlajiUiklg.png)
Validation Accuracy on a 3x3-based Convnet (orange) and the equivalent 5x5-based Convnet (blue)

Also 3 * 3 kernel is easier to use and lighter in construction  and also produces better result with less complications.



# For the pixel of 199 * 199 to reach to 1 * 1 it takes the following approach using 3 * 3 kernel

1. 199 * 199|3 * 3|197 * 197

2. 197 * 197|3 * 3|195 * 195

3. 195 * 195|3 * 3|193 * 193

4. 193 * 193|3 * 3|191 * 191

5. 191 * 191|3 * 3|189 * 189

6. 189 * 189|3 * 3|187 * 187

7. 187 * 187|3 * 3|185 * 185

8. 185 * 185|3 * 3|183 * 183

9. 183 * 183|3 * 3|181 * 181

10. 181 * 181|3 * 3|179 * 179

11. 179 * 179|3 * 3|177 * 177

12. 177 * 177|3 * 3|175 * 175

13. 175 * 175|3 * 3|173 * 173

14. 173 * 173|3 * 3|171 * 171

15. 171 * 171|3 * 3|169 * 169

16. 169 * 169|3 * 3|167 * 167

17. 167 * 167|3 * 3|165 * 165

18. 165 * 165|3 * 3|163 * 163

19. 163 * 163|3 * 3|161 * 161

20. 161 * 161|3 * 3|159 * 159

21. 159 * 159|3 * 3|157 * 157

22. 157 * 157|3 * 3|155 * 155

23. 155 * 155|3 * 3|153 * 153

24. 153 * 153|3 * 3|151 * 151

25. 151 * 151|3 * 3|149 * 159

26. 149 * 149|3 * 3|147 * 147

27. 147 * 147|3 * 3|145 * 145

28. 145 * 145|3 * 3|143 * 143

29. 143 * 143|3 * 3|141 * 141

30. 141 * 141|3 * 3|139 * 139

31. 139 * 139|3 * 3|137 * 137

32. 137 * 137|3 * 3|135 * 135

33. 135 * 135|3 * 3|133 * 133

34. 133 * 133|3 * 3|131 * 131

35. 131 * 131|3 * 3|129 * 129

36. 129 * 129|3 * 3|127 * 127

37. 127 * 127|3 * 3|125 * 125

38. 125 * 125|3 * 3|123 * 123

39. 123 * 123|3 * 3|121 * 121

40. 121 * 121|3 * 3|119 * 119

41. 119 * 119|3 * 3|117 * 117

42. 117 * 117|3 * 3|115 * 115

43. 115 * 115|3 * 3|113 * 113

44. 113 * 113|3 * 3|111 * 111

45. 111 * 111|3 * 3|109 * 109

46. 109 * 109|3 * 3|107 * 107

47. 107 * 107|3 * 3|105 * 105

48. 105 * 105|3 * 3|103 * 103

49. 103 * 103|3 * 3|101 * 101

50. 101 * 101|3 * 3|99 * 99

51. 99 * 99|3 * 3|97 * 97

52. 97 * 97|3 * 3|95 * 95

53. 95 * 95|3 * 3|93 * 93

54. 93 * 93|3 * 3|91 * 91

55. 91 * 91|3 * 3|89 * 89

56. 89 * 89|3 * 3|87 * 87

57. 87 * 87|3 * 3|85 * 85

58. 85 * 85|3 * 3|83 * 83

59. 83 * 83|3 * 3|81 * 81

60. 81 * 81|3 * 3|79 * 79

61. 79 * 79|3 * 3|77 * 77

62. 77 * 77|3 * 3|75 * 75

63. 75 * 75|3 * 3|73 * 73

64. 73 * 73|3 * 3|71 * 71

65. 71 * 71|3 * 3|69 * 69

66. 69 * 69|3 * 3|67 * 67

67. 67 * 67|3 * 3|65 * 65

68. 65 * 65|3 * 3|63 * 63

69. 63 * 63|3 * 3|61 * 61

70. 61 * 61|3 * 3|59 * 59

71. 59 * 59|3 * 3|57 * 57

72. 57 * 57|3 * 3|55 * 55
 
73. 55 * 55|3 * 3|53 * 53

74. 53 * 53|3 * 3|51 * 51

75. 51 * 51|3 * 3|49 * 49

76. 49 * 49|3 * 3|47 * 47

77. 47 * 47|3 * 3|45 * 45

78. 45 * 45|3 * 3|43 * 43

79. 43 * 43|3 * 3|41 * 41

80. 41 * 41|3 * 3|39 * 39

81. 39 * 39|3 * 3|37 * 37

82. 37 * 37|3 * 3|35 * 35

83. 35 * 35|3 * 3|33 * 33

84. 33 * 33|3 * 3|31 * 31

85. 31 * 31|3 * 3|29 * 29

86. 29 * 29|3 * 3|27 * 27

87. 27 * 27|3 * 3|25 * 25

88. 25 * 25|3 * 3|23 * 23

89. 23 * 23|3 * 3|21 * 21

90. 21 * 21|3 * 3|19 * 19

91. 19 * 19|3 * 3|17 * 17

92. 17 * 17|3 * 3|15 * 15 

93. 15 * 15|3 * 3|13 * 13

94. 13 * 13|3 * 3|11 * 11

95. 11 * 11|3 * 3|9 * 9

96. 9 * 9|3 * 3|7 * 7

97. 7 * 7|3 * 3|5 * 5

98. 5 * 5|3 * 3|3 * 3

99. 3 * 3|3 * 3|1 * 1

# Therfore from the above statements we see that 3 * 3 convolution should be performed 99 times on 199 * 199 to get 1*1 ! 
