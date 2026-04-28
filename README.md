backend/models
const ItemSchema = new mongoose.Schema({
    name: { type: String, required: true },
    price: {type: Number, required: true},
    discountPercentage: {type: Number, required: true}
    
}, { timestamps: true });

backend/routes
// POST create item
router.post('/', async (req, res) => {
  const item = new Item({
    name: req.body.name,
    price: req.body.price,
    discountPercentage: req.body.discountPercentage
    // will work once you add price to the model
  });

frontend/components/


Github Commands
echo "# aa" >> README.md
git init
git add README.md
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/IT24101938/Dep_Test.git
git push -u origin main
