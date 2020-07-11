<tamplate>
    <div>
        <span> {{ randomNumber }}</span>
        <button @click="generateRandom">Click to generate</button>
    </div>
</tamplate>

<script>
    export default {
        props: {
            min: {
                type: Number,
                default: 1
            },
            max: {
                type: Number,
                default: 10
            }
        },
        data() {
            return {
                randomNumber: 0
            }
        },
        methods: {
            generateRandom() {
                this.randomNumber = Math.floor(Math.random() * (this.max - this.min + 1)) + this.min;
            }
        }
    }
</script>
