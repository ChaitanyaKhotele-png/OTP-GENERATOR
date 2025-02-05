import java.util.Random;

class OTPGenerator {
    // Method to generate a 6-digit OTP
    public static String generateOTP() {
        Random random = new Random();
        int otp = random.nextInt(900000) + 100000;  // Generates a random number between 100000 and 999999
        return String.valueOf(otp);  // Convert OTP to String and return
    }

    public static void main(String[] args) {
        // Generate OTP
        String otp = generateOTP();
        
        // Print the OTP
        System.out.println("Generated OTP: " + otp);
    }
}
