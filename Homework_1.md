### 1_R

In statistics, a statistical population is a set of entities, also known as "units", that can be grouped together by a common feature.
They are subject of study due to some interest questions.  
In ## Descriptive Statistics, # population is the object from where extract informations, in the
other hand in ## Inferential Statistics it can be treat as the means to make inferences about
the population itself.  

### 2_R

In statistics, an attribute is a characteristic that describes an entity (person, thing)
A variable is an attribute that varies according to the nature of the entity.
For example, if we take a person as an example, a variable is gender, since
describes the person (an attribute), but can vary (man, woman).
A dataset is a collection of data that are usually organized in tables, which constitute 
the starting point of statistical analyzes. 
The data comes from a statistical population using various sampling techniques, like
random sampling, probabilistic sampling, judgmental sampling, convenience sampling.  

### 3_R

A univariate dataset is a dataset formed by the collection of data coming from a single variable of a set of statistical units.
Let's take as an example a set of players (X) within a football team and as a variable, take their height, we will obtain a dataset having the heights of each player.
A frequency distribution (histograms, line charts, bar charts and pie charts) instead shows the data in an organized way through a summary of data divided into classes that are mutually exclusive.
For example, we could have a histogram showing the division of the players within the team based on their height.
It is not possible to reconstruct a dataset from a distribution since there is a loss of data when passing from the dataset to the distribution, as the association between units (which make up the set of statistical units) and value is lost.
This event is wanted since we want to maintain data privacy, in fact we do not want an association between
unit and specific value. In this process, information is lost but knowledge is gained.  

### 1_A  

  - [Homework1_vb](https://drive.google.com/file/d/1XcSTwXmfvgKBUramkWeXWAZ4oFv_20_Z/view?usp=sharing)
  - [Homework1_c#](https://drive.google.com/file/d/1mD8ARARhOLO_AHKrU6GJSzjgp76Nyf0q/view?usp=sharing)  

### 2_A

In C # it is possible to pass arguments to a function by value and by reference. When you pass a variable of type value to a method, you pass a copy of the variable to the method.
Passing by reference, on the other hand, allows functions to modify the value of the parameters and make the changes permanent within the calling environment through the "ref" statement. 
As we can see in the code below, when the argument is passed by value no change occurs, while when it is passed by reference the value (arg = 4) within the calling environment is changed (4 * 4 = 16) .  

```
class Program
{
    static void Main(string[] args)
    {
        int arg;

        // Passing by value.
        // The value of arg in Main is not changed.
        arg = 4;
        squareVal(arg);
        Console.WriteLine(arg);
        // Output: 4

        // Passing by reference.
        // The value of arg in Main is changed.
        arg = 4;
        squareRef(ref arg);
        Console.WriteLine(arg);
        // Output: 16
    }

    static void squareVal(int valParameter)
    {
        valParameter *= valParameter;
    }

    // Passing by reference
    static void squareRef(ref int refParameter)
    {
        refParameter *= refParameter;
    }
} 
```

Also in VB.Net it is possible to pass arguments to a function by value and by reference, respectively
using the ByVal and ByRef commands.
ByVal means that you are passing a copy of a variable, while ByRef does not pass a copy but a pointer to the
original variable. With ByRef the calling procedure can therefore modify the variable and its members.

```
Public Class Simple
    Sub Main()
        Dim value As Integer = 1

        // The integer value doesn't change here when passed ByVal.
        test_val(value)
        Console.WriteLine(value) // OUTPUT 1

        // The integer value DOES change when passed ByRef.
        test_ref(value)
        Console.WriteLine(value)  // OUTPUT 10
    End Sub

    Sub test_val(ByVal test As Integer)
        test = 10
    End Sub

    Sub test_ref(ByRef test As Integer)
        test = 10
    End Sub
End Class 
```

### 1_RA 

In C # to respond to an event you need to define an event handler method (richTextBox1_DragDrop
in the previous exercise) within the function that takes care of receiving events (UserControl1).
In the event handler you define the necessary actions that must be performed when the event is raised.
In VB, the Handles keyword is used when defining a function to specify that function
handles a particular event, the AddHandler keyword is used for
associate an event with an event handler at run time. Personally it seems more comfortable and intuitive to me
event management in VB.Net, but in general the syntax of c # is similar to other programming languages I know, so I will probably use it.  

### 2_RA

The two files have a similar role, they constitute the entry point of the programs: As is clearly explained in the Program.cs file by a self-generated comment.

```
using DevExpress.XtraEditors;
using System;
using System.Windows.Forms;

namespace WindowsFormsApplication1 {
    static class Program {
        /// <summary>
        /// The main entry point for the application.
        /// </summary>
        [STAThread]
        static void Main() {
            //Add your code here
            WindowsFormsSettings.ForceDirectXPaint();
            WindowsFormsSettings.EnableFormSkins();

            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            Application.Run(new Form1());
        }
    }
}
```

The Application.Designer.vb file contains the "Myapplication" class:

```
Partial Friend Class MyApplication

        <Global.System.Diagnostics.DebuggerStepThroughAttribute()> _
        Public Sub New()
            MyBase.New(Global.Microsoft.VisualBasic.ApplicationServices.AuthenticationMode.Windows)
            Me.IsSingleInstance = false
            Me.EnableVisualStyles = true
            Me.SaveMySettingsOnExit = true
            Me.ShutDownStyle = Global.Microsoft.VisualBasic.ApplicationServices.ShutdownMode.AfterMainFormCloses
        End Sub

        <Global.System.Diagnostics.DebuggerStepThroughAttribute()> _
        Protected Overrides Sub OnCreateMainForm()
            Me.MainForm = Global.Homework1_VB.Form1
        End Sub
    End Class
```    

The OnCreateMainForm method establishes which window must be the startup one (Homework_1VB), while Form1 is the default name that Visual Studio assigns to the main window when a new project is created.









### Sources
  https://www.informit.com/articles/article.aspx?p=1602817&seqNum=3
  https://en.wikipedia.org/wiki/Statistical_population
