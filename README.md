# gridbaglayout


import java.awt.*;

class GBLayout extends Frame
{   
    GridBagLayout gbl=new GridBagLayout();
	GBLayout()
	{
		setSize(500,500);
		setLayout(gbl);
		setVisible(true);
		
		GridBagConstraints gbc=new GridBagConstraints();
		
		Button b1=new Button("b1");
		Button b2=new Button("b2");
		Button b3=new Button("b3");
		Button b4=new Button("b4");
		Button b5=new Button("b5");
		
		
		gbc.gridx=0;
		gbc.gridy=0;
		add(b1,gbc);
		
		gbc.gridx=1;
		gbc.gridy=0;
		add(b2,gbc);
		
		gbc.gridx=0;
		gbc.gridy=1;
		add(b3,gbc);
		
		gbc.gridx=1;
		gbc.gridy=1;
		add(b4,gbc);
		
		gbc.gridx=0;
		gbc.gridy=2;
		gbc.fill=GridBagConstraints.VERTICAL;
		gbc.gridwidth=2;
		add(b5,gbc);
			
	}
	
	public static void main(String args[])
	{
		new GBLayout();
	}
}
