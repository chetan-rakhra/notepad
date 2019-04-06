# notepad
import java.awt.Frame;
import java.awt.MenuBar;
import java.awt.Menu;
import java.awt.MenuItem;
import java.awt.TextArea;

class notepad
{
	void func()
	{
		Frame f1=new Frame("myNotepaD");
		MenuBar mb=new MenuBar();


		Menu m1 = new Menu("File");
		Menu m2 = new Menu("Edit");
		Menu m3 = new Menu("Format");
		Menu m4 = new Menu("View");
		Menu m5 = new Menu("Help");

		MenuItem m11 = new MenuItem("New");
		MenuItem m12 = new MenuItem("Open");
		MenuItem m13 = new MenuItem("Save");				
		MenuItem m14 = new MenuItem("Save As..");
		MenuItem m15 = new MenuItem("Page Setup");
		MenuItem m16 = new MenuItem("Print");
		MenuItem m17 = new MenuItem("Exit");

		MenuItem m21 = new MenuItem("Undo");
		MenuItem m22 = new MenuItem("Cut");
		MenuItem m23 = new MenuItem("Copy");				
		MenuItem m24 = new MenuItem("Paste");
		MenuItem m25 = new MenuItem("Delete");
		MenuItem m26 = new MenuItem("Find");
		MenuItem m27 = new MenuItem("Find Next");
		MenuItem m28 = new MenuItem("Replace");
		MenuItem m29 = new MenuItem("Goto");
		MenuItem m210 = new MenuItem("Select all");
		MenuItem m211 = new MenuItem("Time/date");

		MenuItem m31 = new MenuItem("WordWrap");
		MenuItem m32 = new MenuItem("Font");

		MenuItem m41 = new MenuItem("Status Bar");

		MenuItem m51 = new MenuItem("View Help");
		MenuItem m52 = new MenuItem("About Notepad");

		TextArea ta = new TextArea();

		f1.setMenuBar(mb);
		mb.add(m1);
		mb.add(m2);
		mb.add(m3);
		mb.add(m4);
		mb.add(m5);

		m1.add(m11);
		m1.add(m12);
		m1.add(m13);
		m1.add(m14);
		m1.add(m15);
		m1.add(m16);
		m1.add(m17);

		m2.add(m21);
		m2.add(m22);
		m2.add(m23);
		m2.add(m24);
		m2.add(m25);
		m2.add(m26);
		m2.add(m27);
		m2.add(m28);
		m2.add(m29);
		m2.add(m210);
		m2.add(m211);
		
		m3.add(m31);
		m3.add(m32);

		m4.add(m41);
		
		m5.add(m51);
		m5.add(m52);

		f1.add(ta);
		
		f1.setVisible(true);
		f1.setSize(400,500);

		f1.setLocationRelativeTo(null);
	}
	public static void main(String args[])
	{
		notepad obj=new notepad();
		obj.func();
	}
}

