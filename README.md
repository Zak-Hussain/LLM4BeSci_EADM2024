## LLM4BeSci_EADM2024

This course introduces the use of open-source large language models (LLMs) from the Hugging Face ecosystem for research in the behavioral.

By [Zak Hussain](https://zak-hussain.github.io/) and [Dirk Wulff](https://www.mpib-berlin.mpg.de/person/93374/2549)

### Schedule

#### Workshop 1 (Monday)

13:30 - 14:00: Talk: A gentle introduction to Hugging Face and Python<br>
14:00 - 14:45: Exercise:  Pipelines and APIs<br>
14:45 - 15:00: Walkthrough<br>

#### Workshop 2 (Tuesday)

09:00 - 09:30: Talk: Intro to embeddings<br>
09:30 - 10:15: Exercise: Clarifying personality psychology<br>
10:15 - 10:30: Walkthrough<br>

#### Workshop 3 (Tuesday)

11:00 - 11:30: Talk: Intro to text generation<br>
11:30 - 12:15: Exercise: Labeling and synthetic participants<br>
12:15 - 12:30: Walkthrough<br>

### Additional Resources

<a href="https://doi.org/10.3758/s13428-024-02455-8">Hussain, Z., Binz, M., Mata, R., & Wulff, D. U. (2024). A tutorial on open-source large language models for behavioral science. *Behavior Research Methods*, 1-24.
</a>

Bibtex citation:

```
@article{hussain2024tutorial,
  title={A tutorial on open-source large language models for behavioral science},
  author={Hussain, Zak and Binz, Marcel and Mata, Rui and Wulff, Dirk U},
  journal={Behavior Research Methods},
  pages={1--24},
  year={2024},
  publisher={Springer}
}
```

### Installation Instructions
0. If you do not have a Google account, you will need to create one (this can be deleted after the workshop).
1. Navigate to Google Drive (https://drive.google.com/).
2. In the top-left, click New > More > Colaboratory. If you do not see Colaboratory, you may need to click "Connect more apps", 
search for 'Colaboratory', and install it. Then click New > More > Colaboratory.
3. Copy the following code snipped into the first cell of the notebook. Run it (```shift + enter``` or click &#9658; button) to mount your Google Drive to the Colab environment.
A pop-up will ask you to connect; click through the steps to connect your Google Drive to Colab (you will have to do this
every time you open a new notebook).
```
from google.colab import drive
drive.mount("/content/drive")
```
4. Create a second cell in your notebook using the "+ Code" button that appears when you hover your cursor right under the first cell. Copy and run the following code snippet in the second cell of your notebook to clone the GitHub repository to your Google Drive :
```
%cd /content/drive/MyDrive
!git clone https://github.com/Zak-Hussain/LLM4BeSci_EADM2024.git
```
5. Go back to your Google Drive and navigate to the folder "LLM4BeSci_EADM2024". You should see the relevant notebook (ending `.ipynb`) and data files in each folder (it may take  a couple of minutes for the files to appear).

#### Hugging Face API Setup Instructions
The following steps are required to access the Llama-3 model via the Hugging Face API, which we will use in the workshop.

6. Make sure you have a Hugging Face account (https://huggingface.co/join) (it's free!). 
7. Go to the [Llama-3 model page](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct) and fill in the 'META LLAMA 3 COMMUNITY LICENSE AGREEMENT' form at the top of the page in order to get access to the model (this can take up to an hour). 
8. Once you have received an email from Hugging Face saying that you have been granted access, you can navigate to [your Hugging Face profile settings](https://huggingface.co/settings/tokens) to generate an API access token. Click 'New token' at the bottom of the page, give your token a name, and select  'Type'='Read'. This token should provide access to all models in the Llama family. 
