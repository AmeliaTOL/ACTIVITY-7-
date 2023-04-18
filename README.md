# HOMEWORK-7-
Actividad 7
use Illuminate\Database\Seeder;
use App\User;
use App\RoboticsKit;

class NombredetuSembradora extends Seeder
{
    public function run()
    {
        // Crear usuario Admón.
        User::create([
            'name' => 'Admón.',
            'email' => 'admon@robotics.com',
            'password' => bcrypt('Adm@2022'),
            'role' => 'Administrativo'
        ]);

        // Crear usuario Tecmilenio.
        User::create([
            'name' => 'Tecmilenio',
            'email' => 'tecmilenio@robotics.com',
            'password' => bcrypt('Adm@2022'),
            'role' => 'Profesor'
        ]);

        // Crear usuario Estudiante.
        User::create([
            'name' => 'Estudiante',
            'email' => 'estudiante@robotics.com',
            'password' => bcrypt('Adm@2022'),
            'role' => 'Estudiante'
        ]);

        // Crear kit de robótica StarterKit.
        RoboticsKit::create([
            'kit_name' => 'StarterKit'
        ]);

        // Crear kit de robótica Educational Robotics Kit.
        RoboticsKit::create([
            'kit_name' => 'Educational Robotics Kit'
        ]);

        // Crear kit de robótica Kit5.
        RoboticsKit::create([
            'kit_name' => 'Kit5'
        ]);
    }
}
