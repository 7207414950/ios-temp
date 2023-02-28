# ios-temp
import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var Image: UIImageView!
    
    @IBOutlet weak var input: UITextField!
    
    @IBOutlet weak var label: UILabel!
    
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view.
    }

    @IBAction func ClickMe(_ sender: UIButton) {
        var temp = Double(input.text!)!
        if(temp<5){
            Image.image = UIImage(named: "Winter")
            label.text! = "Its soo Cool"
        }
        else if(temp>5 && temp<24){
            Image.image = UIImage(named: "Sun")
            label.text! = "Its Warm"
        }
        else{
            Image.image = UIImage(named: "Hot")
            label.text! = "Its Hot"
        }
    }
    
}
