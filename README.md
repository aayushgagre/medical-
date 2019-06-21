System.out.println("Enter the designation of the employee");

				while (true) {
					String s_desig = br.readLine();
					boolean ch1 = Validator.validateDesignation(salary, s_desig);
					if (ch1 == true) {
						try {
							desig = s_desig;
							break;
						} catch (Exception e) {
							System.out.println("Designation is not correct");
							e.printStackTrace();
						}
					} else
						System.out.println("Designation is  not correct as per salary. Please Re enter the designatio");
				}
