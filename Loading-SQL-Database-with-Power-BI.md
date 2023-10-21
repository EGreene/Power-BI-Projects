Here is how to use Power BI on Windows to load a SQL Server database running on a Linux virtual machine.

Before you do this, make sure you have started your virtual machine on Linux with Microsoft SQL Server running.

When you start the program, you will have multiple options for adding data to your report.

Choose "Import data from SQL Server."

![image](https://github.com/EGreene/Power-BI-Projects/assets/145801984/550f137c-cecb-4827-b471-b1274cf3f999)

Enter the server name: Here, I use the Linux command ```hostname```

My hostname is ```localhost.localdomain```  .
I copy that into the Server field in Power BI.

In the "database(optional)" field, you can put in the database name if you would like. I know the name of the database being used is "HR", so I will insert it there.

![image](https://github.com/EGreene/Power-BI-Projects/assets/145801984/d5f72c02-b056-43f2-9a02-874028b5d6ef)

If this does not get you to the next step, may need to go to Linux and use ```firewall-cmd``` to add a port that may be otherwise blocked.

You may also be asked for a username and password. Remember the username and password you use to log on to Microsoft SQL Server.

Now, you will see a list of tables to use:

![image](https://github.com/EGreene/Power-BI-Projects/assets/145801984/bba264a0-e357-432e-a383-f96ecd05b625)

Select all tables and choose to transform data. Review everything, and click "Close & Apply" on the upper left.

Click on the "Model View" tab, third from the top on the left sidebar, to see the various tables and their relationship.

![image](https://github.com/EGreene/Power-BI-Projects/assets/145801984/0784da40-23f3-460b-b063-386d3b14d4bc)

Then, right click on the link between employees and dependents, and click properties. There can be multiple dependents for one employee, so the relationship between employees and dependents, is one to many, or many dependents to one employee.

![image](https://github.com/EGreene/Power-BI-Projects/assets/145801984/8414ebcf-4b42-45b2-8034-77de8c319476)

Now, we can click on the "Report View" tab, and we are ready to start making reports. See the Power BI files I have uploaded for more information.


