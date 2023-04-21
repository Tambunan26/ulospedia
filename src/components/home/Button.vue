<template>
    <div>
        <button class="baseButton default">{{ buttonText }}</button>
    </div>
</template>
<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'button',
    props:{
        buttonText:{
            type: String,
            default:()=>"Label"
        }
    }
}
</script>

<style scoped>
.baseButton {
  border: none;
  cursor: pointer;
  font-weight: 500;
  color: white;
  background: #3355B5;
  align-items: center;
  padding: 8px 16px;
  font-size: 16px;
  justify-content: center;
  border-radius: 8px;
}

.baseButton.small {
  padding: 8px;
  font-size: 12px;
  border-radius: 4px;
}

/* .baseButton.medium {
  padding: 8px 16px;
  font-size: 16px;
} */

.baseButton.large {
  padding: 8px 16px;
  font-size: 18px;
}

.baseButton:hover {
  background: #2A4797;
}

.baseButton:active {
  background: #192A5A;
}

.baseButton:focus {
  outline: none;
  box-shadow: 0 0 0 3px rgba(51, 85, 181, 0.3);
}

.baseButton:disabled {
  background: rgba(51, 85, 181, 0.2);
  cursor: not-allowed;
}

</style>