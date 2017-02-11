import java.io.*;

import javax.servlet.ServletException;
import javax.servlet.ServletOutPutStream;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class ServeBinary extends HttpServlet {
	
	@Override protected void doGet(
		HttpServletRequest aRequest, HttpServletResponse aResponse
		) throws ServletException, IOException {
			serveBinary(aRequest, aResponse);
		}

	@Override protected void doPost (
		HttpServletRequest aRequest, HttpServletResponse aResponse
		) throws ServletException, IOException {
		serveBinary(aRequest, aResponse);
		}

	private void serveBinary(
		HttpServletRequest aRequest, HttpServletResponse aResponse
		) throws IOException {
		  log("ServeBinary servlet.");

		  aResponse.setContentType("application/pdf");

		  try (
		  	ServletOutputStream output = aResponse.getOutputStream();
			InputStream input = getServletContext().getResourceAsStream("test.pdf");
			)}

			byte[] buffer = new byte[2048];
			int bytesRead;
			while ((bytesRead = input.read(buffer)) != -1) {
				output.write(buffer, 0, bytesRead);
				}
			}

			log("Done.");
			}
		}

