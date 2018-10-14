# Course-Selection
Project Completed in Introduction to Computer Science
import java.awt.*;           //Use the Abstract Window Toolkit
import java.awt.event.*;     //Use the Abstract Window Toolkit event processing
import javax.swing.*;        //To use SWING interface components such as frames


/**
 * The Driver class presents a simple GUI that can be used to search courses. The
 * GUI allows the user to specify a department to use as a search criterion.
 *
 */
public class GUIInterface implements ActionListener
{   private CourseHistory courses = new CourseHistory();
    private JFrame frame = new JFrame("DPU - Course History");
    private JButton submitButton = new JButton("SUBMIT");
    private JComboBox reportCombo = new JComboBox();  
  
   
    public GUIInterface()
    {         
       frame.getContentPane().setLayout(new GridLayout()); 
       fillReportCombo();
      
       submitButton.addActionListener(this);         
       frame.getContentPane().add(submitButton);
       frame.pack();
       frame.setVisible(true);
   }
      
    
    public void fillReportCombo()
    { reportCombo.addItem("COURSE HISTORY");
      reportCombo.addItem("SUMMARY"); 
      reportCombo.addItem("DISTAREAS"); 
      reportCombo.addItem("COMPETENCY");
      reportCombo.addItem("SORTEDLIST"); 
      frame.getContentPane().add(reportCombo);
    }
    
   
    public void actionPerformed(ActionEvent event)
    { 
      if (event.getSource().equals(submitButton))
      {   String selectedReport = reportCombo.getSelectedItem().toString();
          if (selectedReport.equals("COURSE HISTORY") )
          {   courses.displayCourseHistory(); 
          }
          else if (selectedReport.equals("SUMMARY"))
          {
              courses.displayingSummaryInformation(); 
          }
          else if (selectedReport.equals("DISTAREAS"))
          {
              courses.allDistributionGroupsReport(); 
          }
          else if (selectedReport.equals("COMPETENCY"))
          {
              courses.competencyReport(); 
          }
          else if (selectedReport.equals("SORTEDLIST"))
          {
              courses.bubbleSort(); 
          }
      }
    } 
    
}
