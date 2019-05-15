## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/lingxir/lingxir.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/lingxir/lingxir.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

public class NoteEditText extends EditText {
 
    private Context context;
    private boolean initialized;
    // 画笔 用来画下划线
    private Paint paint;
    private Paint mNumPaint;
    private Paint mRectPaint;
    private int mNumberLength;
    private float mTextSize; // sp
 
    private ScrollView mScrollView;
 
    public static final String KEY_TEXT_SIZE = "textSize";
    private String KEY_NUMBER_LENGTH = "_numberLength";
    public static final String KEY_SHOW_LINE = "showLine";
    public static final String KEY_SHOW_LINE_NUMBER = "showLineNumber";
 
    public static final float DEFAULT_VALUE_TEXT_SIZE = 20;
    public static final boolean DEFAULT_VALUE_SHOW_LINE = true;
    public static final boolean DEFAULT_VALUE_SHOW_LINE_NUMBER = false;
    private boolean showLine;
    private boolean showLineNumber;
 
    private int mPaddingLeft;
 
    private static final int LINE_OFFSET = 50;
 
    float displayPaddingLeft;
 
    public NoteEditText(Context context, AttributeSet attrs
