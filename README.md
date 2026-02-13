<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Class 10 Computer - Arrays | Important Questions</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            overflow: hidden;
        }

        header {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 30px;
            text-align: center;
        }

        header h1 {
            font-size: 2em;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.1em;
            opacity: 0.9;
        }

        .content {
            padding: 30px;
        }

        .section {
            margin-bottom: 30px;
        }

        .section-title {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 15px 20px;
            border-radius: 10px;
            font-size: 1.3em;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .question-card {
            background: #f8f9fa;
            border-left: 4px solid #f093fb;
            padding: 20px;
            margin-bottom: 15px;
            border-radius: 8px;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .question-card:hover {
            background: #e9ecef;
            transform: translateX(5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .question {
            font-weight: 600;
            color: #333;
            margin-bottom: 10px;
            font-size: 1.05em;
        }

        .marks {
            display: inline-block;
            background: #f5576c;
            color: white;
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 0.85em;
            margin-left: 10px;
        }

        .answer {
            display: none;
            margin-top: 15px;
            padding: 15px;
            background: white;
            border-radius: 5px;
            color: #555;
            line-height: 1.6;
        }

        .answer.show {
            display: block;
            animation: slideDown 0.3s ease;
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-10px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .toggle-btn {
            background: #f093fb;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.9em;
            margin-top: 10px;
            transition: background 0.3s ease;
        }

        .toggle-btn:hover {
            background: #e082ea;
        }

        code {
            background: #f4f4f4;
            padding: 2px 6px;
            border-radius: 3px;
            font-family: 'Courier New', monospace;
            color: #d63384;
        }

        .code-block {
            background: #2d2d2d;
            color: #f8f8f2;
            padding: 15px;
            border-radius: 5px;
            overflow-x: auto;
            margin: 10px 0;
            font-family: 'Courier New', monospace;
        }

        .note {
            background: #d1ecf1;
            border-left: 4px solid #0c5460;
            padding: 15px;
            margin: 20px 0;
            border-radius: 5px;
        }

        .note strong {
            color: #0c5460;
        }

        ul, ol {
            margin-left: 20px;
            margin-top: 10px;
        }

        li {
            margin-bottom: 8px;
        }

        footer {
            background: #2d3436;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
        }

        .expand-all {
            text-align: center;
            margin: 20px 0;
        }

        .expand-all button {
            background: #28a745;
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1em;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .expand-all button:hover {
            background: #218838;
            transform: scale(1.05);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }

        th {
            border: 1px solid #ddd;
            padding: 10px;
            background: #f093fb;
            color: white;
        }

        td {
            border: 1px solid #ddd;
            padding: 10px;
        }

        .array-visual {
            background: #fff;
            border: 2px solid #f093fb;
            padding: 15px;
            margin: 10px 0;
            border-radius: 5px;
            text-align: center;
        }

        .array-box {
            display: inline-block;
            border: 2px solid #333;
            padding: 10px 15px;
            margin: 2px;
            background: #f8f9fa;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>📚 Class 10 Computer Science</h1>
            <p>Chapter 2: Arrays</p>
            <p style="font-size: 0.9em; margin-top: 10px;">Important Questions & Answers</p>
        </header>

        <div class="content">
            <div class="expand-all">
                <button onclick="toggleAll()">Show All Answers</button>
            </div>

            <!-- Very Short Answer Questions -->
            <div class="section">
                <div class="section-title">
                    📝 Very Short Answer Questions (1 Mark)
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q1. What is an array?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        An array is a collection of similar data elements stored in contiguous memory locations under a single name. All elements in an array must be of the same data type.
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q2. What is the index of the first element in an array?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        The index of the first element in an array is <strong>0 (zero)</strong>. Array indexing starts from 0 in C language.
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q3. What is a subscript in an array?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        A subscript (also called index) is a number used to refer to a particular element in an array. It is written in square brackets [ ]. For example, in <code>marks[3]</code>, 3 is the subscript.
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q4. Write the syntax to declare a one-dimensional array.
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        <strong>Syntax:</strong> <code>data_type array_name[size];</code>
                        <br><br>
                        <strong>Example:</strong> <code>int marks[5];</code>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q5. What are the types of arrays?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        Arrays are of two types:
                        <ul>
                            <li><strong>One-dimensional array</strong> (1D array)</li>
                            <li><strong>Two-dimensional array</strong> (2D array or Multi-dimensional array)</li>
                        </ul>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q6. How do you access the 5th element of an array named 'num'?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        <code>num[4]</code> - Because array indexing starts from 0, the 5th element is at index 4.
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q7. What is array initialization?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        Array initialization means assigning values to array elements at the time of declaration.
                        <br><br>
                        <strong>Example:</strong> <code>int arr[5] = {10, 20, 30, 40, 50};</code>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q8. Can we store elements of different data types in a single array?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        <strong>No</strong>, we cannot store elements of different data types in a single array. All elements must be of the same data type.
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q9. What is a two-dimensional array?
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        A two-dimensional array is an array of arrays, which can be visualized as a table with rows and columns. It requires two subscripts - one for row and one for column.
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q10. Write the declaration of a 2D array with 3 rows and 4 columns.
                        <span class="marks">1 Mark</span>
                    </div>
                    <div class="answer">
                        <code>int arr[3][4];</code>
                        <br><br>
                        This declares a 2D array with 3 rows and 4 columns, having total 12 elements.
                    </div>
                </div>
            </div>

            <!-- Short Answer Questions -->
            <div class="section">
                <div class="section-title">
                    ✍️ Short Answer Questions (2-3 Marks)
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q11. Write the advantages of arrays.
                        <span class="marks">3 Marks</span>
                    </div>
                    <div class="answer">
                        <strong>Advantages of Arrays:</strong>
                        <ul>
                            <li><strong>Easy to use:</strong> Arrays allow storing multiple values under one name</li>
                            <li><strong>Random Access:</strong> Any element can be accessed directly using its index</li>
                            <li><strong>Memory efficient:</strong> Elements are stored in contiguous memory locations</li>
                            <li><strong>Sorting and searching:</strong> Easy to implement sorting and searching algorithms</li>
                            <li><strong>Multiple data handling:</strong> Can handle large amounts of similar data efficiently</li>
                            <li><strong>Code optimization:</strong> Reduces code length and improves performance</li>
                        </ul>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q12. Write the disadvantages of arrays.
                        <span class="marks">2 Marks</span>
                    </div>
                    <div class="answer">
                        <strong>Disadvantages of Arrays:</strong>
                        <ul>
                            <li><strong>Fixed size:</strong> Size of array must be declared in advance and cannot be changed</li>
                            <li><strong>Same data type:</strong> Can store only elements of the same data type</li>
                            <li><strong>Memory wastage:</strong> If array is not completely filled, memory is wasted</li>
                            <li><strong>Insertion/Deletion:</strong> Difficult to insert or delete elements in between</li>
                            <li><strong>Contiguous memory:</strong> Requires continuous memory allocation</li>
                        </ul>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q13. Explain how to declare and initialize a one-dimensional array with example.
                        <span class="marks">3 Marks</span>
                    </div>
                    <div class="answer">
                        <strong>Declaration of Array:</strong>
                        <div class="code-block">
Syntax: data_type array_name[size];

Example:
int marks[5];      // Declares an integer array of size 5
float temp[10];    // Declares a float array of size 10
char name[20];     // Declares a character array of size 20
                        </div>

                        <strong>Initialization of Array:</strong>
                        <div class="code-block">
// Method 1: Initialize at declaration
int marks[5] = {85, 90, 78, 92, 88};

// Method 2: Partial initialization
int num[5] = {10, 20}; // Remaining elements will be 0

// Method 3: Without size (compiler calculates)
int arr[] = {1, 2, 3, 4, 5}; // Size automatically becomes 5

// Method 4: Initialize after declaration
int marks[5];
marks[0] = 85;
marks[1] = 90;
marks[2] = 78;
                        </div>

                        <div class="array-visual">
                            <strong>Array Visualization: marks[5] = {85, 90, 78, 92, 88}</strong><br><br>
                            <div class="array-box">85</div>
                            <div class="array-box">90</div>
                            <div class="array-box">78</div>
                            <div class="array-box">92</div>
                            <div class="array-box">88</div><br>
                            <small>Index: &nbsp;&nbsp;0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4</small>
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q14. Differentiate between one-dimensional and two-dimensional arrays.
                        <span class="marks">3 Marks</span>
                    </div>
                    <div class="answer">
                        <table>
                            <tr>
                                <th>One-Dimensional Array</th>
                                <th>Two-Dimensional Array</th>
                            </tr>
                            <tr>
                                <td>Stores elements in a single row/list</td>
                                <td>Stores elements in rows and columns (table)</td>
                            </tr>
                            <tr>
                                <td>Requires one subscript/index</td>
                                <td>Requires two subscripts (row and column)</td>
                            </tr>
                            <tr>
                                <td>Declaration: <code>int a[5];</code></td>
                                <td>Declaration: <code>int a[3][4];</code></td>
                            </tr>
                            <tr>
                                <td>Access: <code>a[2]</code></td>
                                <td>Access: <code>a[1][2]</code></td>
                            </tr>
                            <tr>
                                <td>Example: List of marks</td>
                                <td>Example: Matrix, table of marks</td>
                            </tr>
                            <tr>
                                <td>Simple structure</td>
                                <td>Complex structure</td>
                            </tr>
                        </table>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q15. How to find the length of an array? Explain with example.
                        <span class="marks">2 Marks</span>
                    </div>
                    <div class="answer">
                        The length of an array can be found using the formula:
                        <br><br>
                        <strong>Length = sizeof(array) / sizeof(array[0])</strong>
                        <br><br>
                        <strong>Example:</strong>
                        <div class="code-block">
#include &lt;stdio.h&gt;

int main()
{
    int arr[] = {10, 20, 30, 40, 50};
    int length;
    
    length = sizeof(arr) / sizeof(arr[0]);
    
    printf("Length of array = %d", length);
    
    return 0;
}

Output: Length of array = 5
                        </div>
                        <strong>Explanation:</strong>
                        <ul>
                            <li><code>sizeof(arr)</code> gives total bytes occupied by array</li>
                            <li><code>sizeof(arr[0])</code> gives bytes occupied by one element</li>
                            <li>Dividing gives the number of elements</li>
                        </ul>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q16. Explain array traversal with example.
                        <span class="marks">3 Marks</span>
                    </div>
                    <div class="answer">
                        <strong>Array Traversal</strong> means accessing each element of an array one by one. This is typically done using loops.
                        <br><br>
                        <strong>Example: Display all elements of an array</strong>
                        <div class="code-block">
#include &lt;stdio.h&gt;

int main()
{
    int arr[5] = {10, 20, 30, 40, 50};
    int i;
    
    printf("Array elements are:\n");
    
    // Traversing using for loop
    for(i = 0; i &lt; 5; i++)
    {
        printf("%d ", arr[i]);
    }
    
    return 0;
}

Output: Array elements are:
        10 20 30 40 50
                        </div>
                        <strong>Explanation:</strong>
                        <ul>
                            <li>Loop starts from i = 0 (first index)</li>
                            <li>Continues till i &lt; 5 (size of array)</li>
                            <li>Each element arr[i] is accessed and printed</li>
                        </ul>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q17. How to declare and initialize a two-dimensional array?
                        <span class="marks">3 Marks</span>
                    </div>
                    <div class="answer">
                        <strong>Declaration of 2D Array:</strong>
                        <div class="code-block">
Syntax: data_type array_name[rows][columns];

Example:
int matrix[3][4];  // 3 rows and 4 columns
float table[2][3]; // 2 rows and 3 columns
                        </div>

                        <strong>Initialization of 2D Array:</strong>
                        <div class="code-block">
// Method 1: Row-wise initialization
int matrix[3][3] = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};

// Method 2: Without inner braces
int arr[2][3] = {10, 20, 30, 40, 50, 60};

// Method 3: Partial initialization
int num[2][2] = {{1, 2}, {3}};
// Result: {{1, 2}, {3, 0}}
                        </div>

                        <strong>Visualization:</strong>
                        <div class="array-visual">
                            matrix[3][3] = {{1,2,3}, {4,5,6}, {7,8,9}}
                            <table style="margin: 10px auto; width: auto;">
                                <tr>
                                    <td style="background: #f093fb; color: white; font-weight: bold;">1</td>
                                    <td style="background: #f093fb; color: white; font-weight: bold;">2</td>
                                    <td style="background: #f093fb; color: white; font-weight: bold;">3</td>
                                </tr>
                                <tr>
                                    <td style="background: #f5576c; color: white; font-weight: bold;">4</td>
                                    <td style="background: #f5576c; color: white; font-weight: bold;">5</td>
                                    <td style="background: #f5576c; color: white; font-weight: bold;">6</td>
                                </tr>
                                <tr>
                                    <td style="background: #f093fb; color: white; font-weight: bold;">7</td>
                                    <td style="background: #f093fb; color: white; font-weight: bold;">8</td>
                                    <td style="background: #f093fb; color: white; font-weight: bold;">9</td>
                                </tr>
                            </table>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Long Answer Questions -->
            <div class="section">
                <div class="section-title">
                    📖 Long Answer Questions (5 Marks)
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q18. Write a C program to find the sum of all elements in a one-dimensional array.
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program to find sum of array elements */
#include &lt;stdio.h&gt;

int main()
{
    int arr[10], n, i, sum = 0;
    
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    
    printf("Enter %d elements:\n", n);
    for(i = 0; i &lt; n; i++)
    {
        scanf("%d", &arr[i]);
    }
    
    // Calculate sum
    for(i = 0; i &lt; n; i++)
    {
        sum = sum + arr[i];
    }
    
    printf("Sum of array elements = %d", sum);
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter the number of elements: 5
Enter 5 elements:
10
20
30
40
50
Sum of array elements = 150
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q19. Write a C program to find the largest element in an array.
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program to find largest element in array */
#include &lt;stdio.h&gt;

int main()
{
    int arr[50], n, i, largest;
    
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    printf("Enter %d elements:\n", n);
    for(i = 0; i &lt; n; i++)
    {
        scanf("%d", &arr[i]);
    }
    
    // Assume first element is largest
    largest = arr[0];
    
    // Compare with remaining elements
    for(i = 1; i &lt; n; i++)
    {
        if(arr[i] &gt; largest)
        {
            largest = arr[i];
        }
    }
    
    printf("Largest element = %d", largest);
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter number of elements: 5
Enter 5 elements:
45
78
23
91
56
Largest element = 91
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q20. Write a C program to search an element in an array (Linear Search).
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program for Linear Search */
#include &lt;stdio.h&gt;

int main()
{
    int arr[50], n, i, search, found = 0;
    
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    printf("Enter %d elements:\n", n);
    for(i = 0; i &lt; n; i++)
    {
        scanf("%d", &arr[i]);
    }
    
    printf("Enter element to search: ");
    scanf("%d", &search);
    
    // Linear search
    for(i = 0; i &lt; n; i++)
    {
        if(arr[i] == search)
        {
            printf("Element %d found at position %d", search, i+1);
            found = 1;
            break;
        }
    }
    
    if(found == 0)
    {
        printf("Element %d not found in array", search);
    }
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter number of elements: 5
Enter 5 elements:
10
20
30
40
50
Enter element to search: 30
Element 30 found at position 3
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q21. Write a C program to sort an array in ascending order (Bubble Sort).
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program for Bubble Sort */
#include &lt;stdio.h&gt;

int main()
{
    int arr[50], n, i, j, temp;
    
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    printf("Enter %d elements:\n", n);
    for(i = 0; i &lt; n; i++)
    {
        scanf("%d", &arr[i]);
    }
    
    // Bubble Sort Algorithm
    for(i = 0; i &lt; n-1; i++)
    {
        for(j = 0; j &lt; n-i-1; j++)
        {
            if(arr[j] &gt; arr[j+1])
            {
                // Swap elements
                temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
    }
    
    printf("Sorted array in ascending order:\n");
    for(i = 0; i &lt; n; i++)
    {
        printf("%d ", arr[i]);
    }
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter number of elements: 5
Enter 5 elements:
64
34
25
12
22
Sorted array in ascending order:
12 22 25 34 64
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q22. Write a C program to find the smallest element in an array.
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program to find smallest element in array */
#include &lt;stdio.h&gt;

int main()
{
    int arr[50], n, i, smallest;
    
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    printf("Enter %d elements:\n", n);
    for(i = 0; i &lt; n; i++)
    {
        scanf("%d", &arr[i]);
    }
    
    // Assume first element is smallest
    smallest = arr[0];
    
    // Compare with remaining elements
    for(i = 1; i &lt; n; i++)
    {
        if(arr[i] &lt; smallest)
        {
            smallest = arr[i];
        }
    }
    
    printf("Smallest element = %d", smallest);
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter number of elements: 5
Enter 5 elements:
45
12
78
23
56
Smallest element = 12
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q23. Write a C program to input and display a 2D array (Matrix).
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program to input and display 2D array */
#include &lt;stdio.h&gt;

int main()
{
    int matrix[10][10], rows, cols, i, j;
    
    printf("Enter number of rows: ");
    scanf("%d", &rows);
    
    printf("Enter number of columns: ");
    scanf("%d", &cols);
    
    printf("Enter elements of matrix:\n");
    for(i = 0; i &lt; rows; i++)
    {
        for(j = 0; j &lt; cols; j++)
        {
            printf("Enter element [%d][%d]: ", i, j);
            scanf("%d", &matrix[i][j]);
        }
    }
    
    printf("\nMatrix is:\n");
    for(i = 0; i &lt; rows; i++)
    {
        for(j = 0; j &lt; cols; j++)
        {
            printf("%d\t", matrix[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter number of rows: 2
Enter number of columns: 3
Enter elements of matrix:
Enter element [0][0]: 1
Enter element [0][1]: 2
Enter element [0][2]: 3
Enter element [1][0]: 4
Enter element [1][1]: 5
Enter element [1][2]: 6

Matrix is:
1    2    3
4    5    6
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q24. Write a C program to add two matrices.
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program to add two matrices */
#include &lt;stdio.h&gt;

int main()
{
    int a[10][10], b[10][10], sum[10][10];
    int rows, cols, i, j;
    
    printf("Enter number of rows: ");
    scanf("%d", &rows);
    
    printf("Enter number of columns: ");
    scanf("%d", &cols);
    
    // Input first matrix
    printf("Enter elements of first matrix:\n");
    for(i = 0; i &lt; rows; i++)
    {
        for(j = 0; j &lt; cols; j++)
        {
            scanf("%d", &a[i][j]);
        }
    }
    
    // Input second matrix
    printf("Enter elements of second matrix:\n");
    for(i = 0; i &lt; rows; i++)
    {
        for(j = 0; j &lt; cols; j++)
        {
            scanf("%d", &b[i][j]);
        }
    }
    
    // Add matrices
    for(i = 0; i &lt; rows; i++)
    {
        for(j = 0; j &lt; cols; j++)
        {
            sum[i][j] = a[i][j] + b[i][j];
        }
    }
    
    // Display result
    printf("\nSum of matrices:\n");
    for(i = 0; i &lt; rows; i++)
    {
        for(j = 0; j &lt; cols; j++)
        {
            printf("%d\t", sum[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter number of rows: 2
Enter number of columns: 2
Enter elements of first matrix:
1 2
3 4
Enter elements of second matrix:
5 6
7 8

Sum of matrices:
6    8
10   12
                        </div>
                    </div>
                </div>

                <div class="question-card" onclick="toggleAnswer(this)">
                    <div class="question">
                        Q25. Write a C program to count even and odd numbers in an array.
                        <span class="marks">5 Marks</span>
                    </div>
                    <div class="answer">
                        <div class="code-block">
/* Program to count even and odd numbers */
#include &lt;stdio.h&gt;

int main()
{
    int arr[50], n, i;
    int even_count = 0, odd_count = 0;
    
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    printf("Enter %d elements:\n", n);
    for(i = 0; i &lt; n; i++)
    {
        scanf("%d", &arr[i]);
    }
    
    // Count even and odd
    for(i = 0; i &lt; n; i++)
    {
        if(arr[i] % 2 == 0)
        {
            even_count++;
        }
        else
        {
            odd_count++;
        }
    }
    
    printf("Even numbers: %d\n", even_count);
    printf("Odd numbers: %d", odd_count);
    
    return 0;
}
                        </div>
                        <strong>Output:</strong>
                        <div class="code-block">
Enter number of elements: 5
Enter 5 elements:
12
15
18
21
24
Even numbers: 3
Odd numbers: 2
                        </div>
                    </div>
                </div>
            </div>

            <div class="note">
                <strong>💡 Important Points to Remember:</strong>
                <ul>
                    <li>Array indexing always starts from 0</li>
                    <li>Array size must be declared at compile time</li>
                    <li>All elements must be of the same data type</li>
                    <li>Arrays are stored in contiguous memory locations</li>
                    <li>For 2D array: Total elements = rows × columns</li>
                    <li>Common operations: Insertion, Deletion, Searching, Sorting, Traversal</li>
                    <li>Practice writing programs for sum, average, largest, smallest elements</li>
                </ul>
            </div>

            <div class="note" style="background: #fff3cd; border-left: 4px solid #ffc107;">
                <strong style="color: #856404;">🎯 Exam Tips:</strong>
                <ul>
                    <li>Always initialize loop variable and array properly</li>
                    <li>Remember: Size of array in declaration, Length in loop condition</li>
                    <li>For 2D arrays, use nested loops (outer for rows, inner for columns)</li>
                    <li>In sorting, practice bubble sort thoroughly</li>
                    <li>For searching, know both linear and binary search</li>
                </ul>
            </div>
        </div>

        <footer>
            <p>📚 Keep practicing array programs! Success awaits! 💪</p>
            <p style="margin-top: 10px; font-size: 0.9em;">Class 10 Computer Science - Chapter 2: Arrays</p>
        </footer>
    </div>

    <script>
        function toggleAnswer(element) {
            const answer = element.querySelector('.answer');
            answer.classList.toggle('show');
        }

        let allExpanded = false;
        function toggleAll() {
            const answers = document.querySelectorAll('.answer');
            const button = document.querySelector('.expand-all button');
            
            if (!allExpanded) {
                answers.forEach(answer => answer.classList.add('show'));
                button.textContent = 'Hide All Answers';
                allExpanded = true;
            } else {
                answers.forEach(answer => answer.classList.remove('show'));
                button.textContent = 'Show All Answers';
                allExpanded = false;
            }
        }
    </script>
</body>
</html>
