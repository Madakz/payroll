# An Online Payroll system

An online payroll system. A personal project developed during my NYSC service

Created By: Madaki Fatsen
Github: Madakz
Time: 9:20pm 2/10/2018

The Login details for the software are:
Username: admin
Password: secret@

Open the class_lib directory, the functions.php file should be open and change the Password of mysql database to your own password

		public function connection()
		{
			try {
			    $hostname ="127.0.0.1";
				$db_username = "root";
				$passwd = "madmyme%%";	//change this password to your mysql password
				$dbname ="payroll";
		        $pdo_obj = new PDO("mysql:host=$hostname;dbname=$dbname", "$db_username", "$passwd");
		        return $pdo_obj;
		     }
		     catch(PDOException $e)
			    {
			    return "Connection failed: " . $e->getMessage();
		    }
		} 
