# Dice-roller-app
import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
import android.view.View
import android.widget.Button
import android.widget.TextView
import android.widget.Toast




class MainActivity : AppCompatActivity() {
    public override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        val rollButton: Button = findViewById(R.id.rollButton)
        rollButton.run({ setOnContextClickListener() })


    }
    private fun rollDice() {
        val dice = Dice(6)
        val diceRoll = dice.roll()
    }

    fun onbuttonclicked(view: View) {}
}
class Dice(private val numSides: Int) {
    fun roll(): Int {
        return (1..numSides).random()
    }
}


private fun TextView.setOnContextClickListener() {
    TODO("Not yet implemented")
}

fun onbuttonclicked(view: View) {



    }

