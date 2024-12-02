import java.awt.*;
import java.awt.event.*;

public class JobPortal extends Frame implements ActionListener {

    // Create components for Job Seeker registration
    Label seekerLabel, nameLabel, emailLabel, resumeLabel;
    TextField nameField, emailField;
    TextArea resumeField;
    Button seekerButton;

    // Create components for Employer job posting
    Label employerLabel, jobTitleLabel, jobDescLabel, jobLocationLabel;
    TextField jobTitleField, jobLocationField;
    TextArea jobDescField;
    Button employerButton;

    // Constructor for setting up the GUI
    public JobPortal() {
        setTitle("Job Portal");
        setSize(500, 400);
        setLayout(new CardLayout());
        
        // Job Seeker Panel
        Panel seekerPanel = new Panel();
        seekerPanel.setLayout(new GridLayout(4, 2));

        seekerLabel = new Label("Job Seeker Registration");
        nameLabel = new Label("Name:");
        emailLabel = new Label("Email:");
        resumeLabel = new Label("Resume:");

        nameField = new TextField();
        emailField = new TextField();
        resumeField = new TextArea();

        seekerButton = new Button("Submit");

        seekerButton.addActionListener(this);

        seekerPanel.add(seekerLabel);
        seekerPanel.add(new Label("")); // Empty cell for alignment
        seekerPanel.add(nameLabel);
        seekerPanel.add(nameField);
        seekerPanel.add(emailLabel);
        seekerPanel.add(emailField);
        seekerPanel.add(resumeLabel);
        seekerPanel.add(resumeField);
        seekerPanel.add(seekerButton);

        // Employer Panel
        Panel employerPanel = new Panel();
        employerPanel.setLayout(new GridLayout(5, 2));

        employerLabel = new Label("Employer Job Posting");
        jobTitleLabel = new Label("Job Title:");
        jobDescLabel = new Label("Job Description:");
        jobLocationLabel = new Label("Location:");

        jobTitleField = new TextField();
        jobLocationField = new TextField();
        jobDescField = new TextArea();

        employerButton = new Button("Post Job");

        employerButton.addActionListener(this);

        employerPanel.add(employerLabel);
        employerPanel.add(new Label("")); // Empty cell for alignment
        employerPanel.add(jobTitleLabel);
        employerPanel.add(jobTitleField);
        employerPanel.add(jobLocationLabel);
        employerPanel.add(jobLocationField);
        employerPanel.add(jobDescLabel);
        employerPanel.add(jobDescField);
        employerPanel.add(employerButton);

        // Adding panels to the frame
        add("seeker", seekerPanel);
        add("employer", employerPanel);

        // Show the Job Seeker Panel by default
        setVisible(true);
    }

    // ActionListener method to handle button clicks
    public void actionPerformed(ActionEvent e) {
        if (e.getSource() == seekerButton) {
            String name = nameField.getText();
            String email = emailField.getText();
            String resume = resumeField.getText();

            // Print registration details to the console
            System.out.println("Job Seeker Registered:");
            System.out.println("Name: " + name);
            System.out.println("Email: " + email);
            System.out.println("Resume: " + resume);

            // Clear fields after submission
            nameField.setText("");
            emailField.setText("");
            resumeField.setText("");
        } else if (e.getSource() == employerButton) {
            String jobTitle = jobTitleField.getText();
            String jobLocation = jobLocationField.getText();
            String jobDesc = jobDescField.getText();

            // Print job posting details to the console
            System.out.println("Job Posted:");
            System.out.println("Job Title: " + jobTitle);
            System.out.println("Location: " + jobLocation);
            System.out.println("Description: " + jobDesc);

            // Clear fields after posting
            jobTitleField.setText("");
            jobLocationField.setText("");
            jobDescField.setText("");
        }
    }

    // Main method to run the application
    public static void main(String[] args) {
        new JobPortal();
    }
}
