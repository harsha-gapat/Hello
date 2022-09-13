# Github API
my second repository in github
import java.text.ParsePosition;
import java.text.SimpleDateFormat;
import java.util.Calendar;
import java.util.Date;

public class Arguments {
	public static void main(String[] args) throws Exception {
		String dt=args[0];

		SimpleDateFormat sdf = new SimpleDateFormat(dt);
		Calendar cal = Calendar.getInstance();

		java.util.Date date = cal.getTime();
		
		System.out.println("Last 10 Days Record");
		
		for (int i = 0; i < 10; i++) {
			cal.add(Calendar.DATE, -1);
		     date = cal.getTime();
			String reportDate = sdf.format(date);

			System.out.println(reportDate);
		
		
		
		
	}

}
}
