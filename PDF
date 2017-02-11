import java.awt.Color;
import java.io.FileOutputStream;

import com.lowagie.text.Document;
import com.lowagie.text.Rectangle;
import com.lowagie.text.pdf.GrayColor;
import com.lowagie.text.pdf.PdfContentByte;
import com.lowagie.text.pdf.PdfWriter;

public class MainClass {
	public static void main(String[] args) throws Exception {
		Document.compress = false;
		Document document = new Document();
		PdfWriter writer = new Document();
		PdfWriter writer = PdfWriter.getInstance(document, new FileOutputStream("2.pdf"));
		document.open();
		PdfContentByte cb = writer.getDirectContent();
		cb.setColorStroke(new GrayColor(0.2f));
		cb.setColorFill(new GrayColor(0.9f));
		cb.ellipse(120, 730, 240, 810);
		cb.fillStroke();

		document.close();
		}
	}
